## Description

<div><p>Malek is a rich man. He also is very generous. That's why he decided to split his money between poor people. A charity institute knows <span class="tex-span"><i>n</i></span> poor people numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The institute gave Malek <span class="tex-span"><i>q</i></span> recommendations. A recommendation is a segment of people like <span class="tex-span">[<i>l</i>, <i>r</i>]</span> which means the institute recommended that Malek gives one dollar to every person whose number is in this segment.</p><p>However this charity has very odd rules about the recommendations. Because of those rules the recommendations are given in such a way that for every two recommendation <span class="tex-span">[<i>a</i>, <i>b</i>]</span> and <span class="tex-span">[<i>c</i>, <i>d</i>]</span> one of the following conditions holds: </p><ul> <li> The two segments are completely disjoint. More formally either <span class="tex-span"><i>a</i> ≤ <i>b</i> &lt; <i>c</i> ≤ <i>d</i></span> or <span class="tex-span"><i>c</i> ≤ <i>d</i> &lt; <i>a</i> ≤ <i>b</i></span> </li><li> One of the two segments are inside another. More formally either <span class="tex-span"><i>a</i> ≤ <i>c</i> ≤ <i>d</i> ≤ <i>b</i></span> or <span class="tex-span"><i>c</i> ≤ <i>a</i> ≤ <i>b</i> ≤ <i>d</i></span>. </li></ul><p>The <span class="tex-font-style-underline">goodness</span> of a charity is the value of maximum money a person has after Malek finishes giving his money. The institute knows for each recommendation what is the probability that Malek will accept it. They want to know the expected value of <span class="tex-font-style-underline">goodness</span> of this charity. So they asked you for help.</p><p>You have been given the list of recommendations and for each recommendation the probability of it being accepted by Malek. You have also been given how much money each person initially has. You must find the expected value of <span class="tex-font-style-underline">goodness</span>.</p></div><div class="input-specification"><p>In the first line two space-separated integers <span class="tex-span"><i>n</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 5000</span>) are given.</p><p>In the second line <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) are given meaning that person number <span class="tex-span"><i>i</i></span> initially has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> dollars. </p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains three space-separated numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>p</i> ≤ 1</span>) where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> are two integers describing the segment of recommendation and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is a real number given with exactly three digits after decimal point which is equal to probability of Malek accepting this recommendation.</p><p>Note that a segment may appear several times in recommendations.</p></div><div class="output-specification"><p>Output the sought value. Your answer will be considered correct if its absolute or relative error is less than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>In the first line two space-separated integers <span class="tex-span"><i>n</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 5000</span>) are given.</p><p>In the second line <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) are given meaning that person number <span class="tex-span"><i>i</i></span> initially has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> dollars. </p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains three space-separated numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>p</i> ≤ 1</span>) where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> are two integers describing the segment of recommendation and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is a real number given with exactly three digits after decimal point which is equal to probability of Malek accepting this recommendation.</p><p>Note that a segment may appear several times in recommendations.</p>

## Output

<p>Output the sought value. Your answer will be considered correct if its absolute or relative error is less than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
5 2
1 7 2 4 3
1 3 0.500
2 2 0.500

```




```input2
5 2
281 280 279 278 282
1 4 1.000
1 4 0.000

```




```input3
3 5
1 2 3
1 3 0.500
2 2 0.250
1 2 0.800
1 1 0.120
2 2 0.900

```




```output1
8.000000000

```




```output2
282.000000000

```




```output3
4.465000000

```


