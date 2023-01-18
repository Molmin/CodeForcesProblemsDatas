## Description

<div><p><span class="tex-font-style-it">In this problem you will have to deal with a real algorithm that is used in the VK social network.</span></p><p>As in any other company that creates high-loaded websites, the VK developers have to deal with request statistics regularly. An important indicator reflecting the load of the site is the mean number of requests for a certain period of time of <span class="tex-span"><i>T</i></span> seconds (for example, <span class="tex-span"><i>T</i> = 60&nbsp;<i>seconds</i> = 1&nbsp;<i>min</i></span> and <span class="tex-span"><i>T</i> = 86400&nbsp;<i>seconds</i> = 1&nbsp;<i>day</i></span>). For example, if this value drops dramatically, that shows that the site has access problem. If this value grows, that may be a reason to analyze the cause for the growth and add more servers to the website if it is really needed.</p><p>However, even such a natural problem as counting the mean number of queries for some period of time can be a challenge when you process the amount of data of a huge social network. That's why the developers have to use original techniques to solve problems approximately, but more effectively at the same time.</p><p>Let's consider the following formal model. We have a service that works for <span class="tex-span"><i>n</i></span> seconds. We know the number of queries to this resource <span class="tex-span"><i>a</i><sub class="lower-index"><i>t</i></sub></span> at each moment of time <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ <i>n</i></span>). Let's formulate the following algorithm <span class="tex-font-style-it">of calculating the mean with exponential decay</span>. Let <span class="tex-span"><i>c</i></span> be some real number, strictly larger than one.</p><pre class="verbatim"><br>// setting this constant value correctly can adjust   <br>// the time range for which statistics will be calculated<br>double c = <span class="tex-font-style-it">some constant value</span>; <br><br>// as the result of the algorithm's performance this variable will contain <br>// the mean number of queries for the last <br>// T seconds by the current moment of time<br>double mean = 0.0; <br><br>for t = 1..n: // at each second, we do the following:<br>    // <span class="tex-span"><i>a</i><sub class="lower-index"><i>t</i></sub></span> is the number of queries that came at the last second;<br>    mean = (mean + <span class="tex-span"><i>a</i><sub class="lower-index"><i>t</i></sub></span> / T) / c;<br></pre><p>Thus, the mean variable is recalculated each second using the number of queries that came at that second. We can make some mathematical calculations and prove that choosing the value of constant <span class="tex-span"><i>c</i></span> correctly will make the value of <span class="tex-font-style-tt">mean</span> not very different from the real mean value <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span> at <span class="tex-span"><i>t</i> - <i>T</i> + 1 ≤ <i>x</i> ≤ <i>t</i></span>. </p><p>The advantage of such approach is that it only uses the number of requests at the current moment of time and doesn't require storing the history of requests for a large time range. Also, it considers the recent values with the weight larger than the weight of the old ones, which helps to react to dramatic change in values quicker.</p><p>However before using the new theoretical approach in industrial programming, there is an obligatory step to make, that is, to test its credibility practically on given test data sets. Your task is to compare the data obtained as a result of the work of an approximate algorithm to the real data. </p><p>You are given <span class="tex-span"><i>n</i></span> values <span class="tex-span"><i>a</i><sub class="lower-index"><i>t</i></sub></span>, integer <span class="tex-span"><i>T</i></span> and real number <span class="tex-span"><i>c</i></span>. Also, you are given <span class="tex-span"><i>m</i></span> moments <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>), where we are interested in the mean value of the number of queries for the last <span class="tex-span"><i>T</i></span> seconds. Implement two algorithms. The first one should calculate the required value by definition, i.e. by the formula <img align="middle" class="tex-formula" src="file://sjQAlIuc.png" style="max-width: 100.0%;max-height: 100.0%;">. The second algorithm should calculate the mean value as is described above. Print both values and calculate the relative error of the second algorithm by the formula <img align="middle" class="tex-formula" src="file://tW68E45u.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>approx</i></span> is the approximate value, obtained by the second algorithm, and <span class="tex-span"><i>real</i></span> is the exact value obtained by the first algorithm.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>), integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ <i>n</i></span>) and real number <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 &lt; <i>c</i> ≤ 100</span>) — the time range when the resource should work, the length of the time range during which we need the mean number of requests and the coefficient <span class="tex-span"><i>c</i></span> of the work of approximate algorithm. Number <span class="tex-span"><i>c</i></span> is given with exactly six digits after the decimal point.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>t</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>t</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the number of queries to the service at each moment of time.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>) — the number of moments of time when we are interested in the mean number of queries for the last <span class="tex-span"><i>T</i></span> seconds.</p><p>The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"><i>T</i> ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>), representing another moment of time for which we need statistics. Moments <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> are strictly increasing.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. The <span class="tex-span"><i>j</i></span>-th line must contain three numbers <span class="tex-span"><i>real</i></span>, <span class="tex-span"><i>approx</i></span> and <span class="tex-span"><i>error</i></span>, where:</p><ul> <li> <img align="middle" class="tex-formula" src="file://6CQn6QhI.png" style="max-width: 100.0%;max-height: 100.0%;"> is the real mean number of queries for the last <span class="tex-span"><i>T</i></span> seconds; </li><li> <span class="tex-span"><i>approx</i></span> is calculated by the given algorithm and equals <span class="tex-span"><i>mean</i></span> at the moment of time <span class="tex-span"><i>t</i> = <i>p</i><sub class="lower-index"><i>j</i></sub></span> (that is, after implementing the <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span>-th iteration of the cycle); </li><li> <img align="middle" class="tex-formula" src="file://bjcOT47Y.png" style="max-width: 100.0%;max-height: 100.0%;"> is the relative error of the approximate algorithm. </li></ul><p>The numbers you printed will be compared to the correct numbers with the relative or absolute error <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>. It is recommended to print the numbers with at least five digits after the decimal point.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>), integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ <i>n</i></span>) and real number <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 &lt; <i>c</i> ≤ 100</span>) — the time range when the resource should work, the length of the time range during which we need the mean number of requests and the coefficient <span class="tex-span"><i>c</i></span> of the work of approximate algorithm. Number <span class="tex-span"><i>c</i></span> is given with exactly six digits after the decimal point.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>t</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>t</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the number of queries to the service at each moment of time.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>) — the number of moments of time when we are interested in the mean number of queries for the last <span class="tex-span"><i>T</i></span> seconds.</p><p>The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"><i>T</i> ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>), representing another moment of time for which we need statistics. Moments <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> are strictly increasing.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. The <span class="tex-span"><i>j</i></span>-th line must contain three numbers <span class="tex-span"><i>real</i></span>, <span class="tex-span"><i>approx</i></span> and <span class="tex-span"><i>error</i></span>, where:</p><ul> <li> <img align="middle" class="tex-formula" src="file://6CQn6QhI.png" style="max-width: 100.0%;max-height: 100.0%;"> is the real mean number of queries for the last <span class="tex-span"><i>T</i></span> seconds; </li><li> <span class="tex-span"><i>approx</i></span> is calculated by the given algorithm and equals <span class="tex-span"><i>mean</i></span> at the moment of time <span class="tex-span"><i>t</i> = <i>p</i><sub class="lower-index"><i>j</i></sub></span> (that is, after implementing the <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span>-th iteration of the cycle); </li><li> <img align="middle" class="tex-formula" src="file://bjcOT47Y.png" style="max-width: 100.0%;max-height: 100.0%;"> is the relative error of the approximate algorithm. </li></ul><p>The numbers you printed will be compared to the correct numbers with the relative or absolute error <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>. It is recommended to print the numbers with at least five digits after the decimal point.</p>





```input1
1 1 2.000000
1
1
1

```




```input2
11 4 1.250000
9 11 7 5 15 6 6 6 6 6 6
8
4 5 6 7 8 9 10 11

```




```input3
13 4 1.250000
3 3 3 3 3 20 3 3 3 3 3 3 3
10
4 5 6 7 8 9 10 11 12 13

```




```output1
1.000000 0.500000 0.500000

```




```output2
8.000000 4.449600 0.443800
9.500000 6.559680 0.309507
8.250000 6.447744 0.218455
8.000000 6.358195 0.205226
8.250000 6.286556 0.237993
6.000000 6.229245 0.038207
6.000000 6.183396 0.030566
6.000000 6.146717 0.024453

```




```output3
3.000000 1.771200 0.409600
3.000000 2.016960 0.327680
7.250000 5.613568 0.225715
7.250000 5.090854 0.297813
7.250000 4.672684 0.355492
7.250000 4.338147 0.401635
3.000000 4.070517 0.356839
3.000000 3.856414 0.285471
3.000000 3.685131 0.228377
3.000000 3.548105 0.182702

```


