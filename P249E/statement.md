## Description

<div><p>A Russian space traveller Alisa Selezneva, like any other schoolgirl of the late 21 century, is interested in science. She has recently visited the MIT (Moscow Institute of Time), where its chairman and the co-inventor of the time machine academician Petrov told her about the construction of a time machine.</p><p>During the demonstration of the time machine performance Alisa noticed that the machine does not have high speed and the girl got interested in the reason for such disadvantage. As it turns out on closer examination, one of the problems that should be solved for the time machine isn't solved by an optimal algorithm. If you find a way to solve this problem optimally, the time machine will run faster and use less energy.</p><p>A task that none of the staff can solve optimally is as follows. There exists a matrix <span class="tex-span"><i>a</i></span>, which is filled by the following rule:</p><p>The cells are consecutive positive integers, starting with one. Besides, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> &lt; <i>a</i><sub class="lower-index"><i>t</i>, <i>k</i></sub></span> (<span class="tex-span"><i>i</i>, <i>j</i>, <i>t</i>, <i>k</i> ≥ 1</span>), if:</p><ol> <li> <span class="tex-span"><i>max</i>(<i>i</i>, <i>j</i>) &lt; <i>max</i>(<i>t</i>, <i>k</i>)</span>; </li><li> <span class="tex-span"><i>max</i>(<i>i</i>, <i>j</i>) = <i>max</i>(<i>t</i>, <i>k</i>)</span> and <span class="tex-span"><i>j</i> &lt; <i>k</i></span>; </li><li> <span class="tex-span"><i>max</i>(<i>i</i>, <i>j</i>) = <i>max</i>(<i>t</i>, <i>k</i>)</span>, <span class="tex-span"><i>j</i> = <i>k</i></span> and <span class="tex-span"><i>i</i> &gt; <i>t</i></span>. </li></ol><p>So, after the first <span class="tex-span">36</span> numbers are inserted, matrix <span class="tex-span"><i>a</i></span> will look as follows:</p><center> <img class="tex-graphics" src="file://rFWQO6ia.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>To solve the problem, you should learn to find rather quickly for the given values of <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub></span>) the meaning of expression:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://zV9myLrI.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>As the meaning of this expression can be large enough, it is sufficient to know only the last <span class="tex-span">10</span> digits of the sought value.</p><p>So, no one in MTI can solve the given task. Alice was brave enough to use the time machine and travel the past to help you.</p><p>Your task is to write a program that uses the given values <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> finds the last <span class="tex-span">10</span> digits of the given expression.</p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of test sets for which you should solve the problem. </p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains the description of a test — four positive integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>), separated by spaces.</p></div><div class="output-specification"><p>For each query print the meaning of the expression if it contains at most <span class="tex-span">10</span> characters. Otherwise, print three characters "<span class="tex-font-style-tt">.</span>" (without the quotes), and then ten last digits of the time expression. Print the answer to each query on a single line. Follow the format, given in the sample as closely as possible.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of test sets for which you should solve the problem. </p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains the description of a test — four positive integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>), separated by spaces.</p>

## Output

<p>For each query print the meaning of the expression if it contains at most <span class="tex-span">10</span> characters. Otherwise, print three characters "<span class="tex-font-style-tt">.</span>" (without the quotes), and then ten last digits of the time expression. Print the answer to each query on a single line. Follow the format, given in the sample as closely as possible.</p>





```input1
5
1 1 1 1
2 2 3 3
2 3 5 6
100 87 288 2002
4 2 5 4

```




```output1
1
24
300
...5679392764
111

```


