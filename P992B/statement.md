## Description

<div><p>Today on Informatics class Nastya learned about GCD and LCM (see links below). Nastya is very intelligent, so she solved all the tasks momentarily and now suggests you to solve one of them as well.</p><p>We define a pair of integers <span class="tex-span">(<i>a</i>, <i>b</i>)</span> <span class="tex-font-style-it">good</span>, if <span class="tex-span"><i>GCD</i>(<i>a</i>, <i>b</i>) = <i>x</i></span> and <span class="tex-span"><i>LCM</i>(<i>a</i>, <i>b</i>) = <i>y</i></span>, where <span class="tex-span"><i>GCD</i>(<i>a</i>, <i>b</i>)</span> denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>LCM</i>(<i>a</i>, <i>b</i>)</span> denotes the <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple</a> of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>You are given two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. You are to find the number of <span class="tex-font-style-it">good</span> pairs of integers <span class="tex-span">(<i>a</i>, <i>b</i>)</span> such that <span class="tex-span"><i>l</i> ≤ <i>a</i>, <i>b</i> ≤ <i>r</i></span>. Note that pairs <span class="tex-span">(<i>a</i>, <i>b</i>)</span> and <span class="tex-span">(<i>b</i>, <i>a</i>)</span> are considered different if <span class="tex-span"><i>a</i> ≠ <i>b</i></span>.</p></div><div class="input-specification"><p>The only line contains four integers <span class="tex-span"><i>l</i>, <i>r</i>, <i>x</i>, <i>y</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In the only line print the only integer&nbsp;— the answer for the problem.</p></div>

## Input

<p>The only line contains four integers <span class="tex-span"><i>l</i>, <i>r</i>, <i>x</i>, <i>y</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In the only line print the only integer&nbsp;— the answer for the problem.</p>





```input1
1 2 1 2

```




```input2
1 12 1 12

```




```input3
50 100 3 30

```




```output1
2

```




```output2
4

```




```output3
0

```



## Note

<p>In the first example there are two suitable <span class="tex-font-style-it">good</span> pairs of integers <span class="tex-span">(<i>a</i>, <i>b</i>)</span>: <span class="tex-span">(1, 2)</span> and <span class="tex-span">(2, 1)</span>.</p><p>In the second example there are four suitable <span class="tex-font-style-it">good</span> pairs of integers <span class="tex-span">(<i>a</i>, <i>b</i>)</span>: <span class="tex-span">(1, 12)</span>, <span class="tex-span">(12, 1)</span>, <span class="tex-span">(3, 4)</span> and <span class="tex-span">(4, 3)</span>.</p><p>In the third example there are <span class="tex-font-style-it">good</span> pairs of integers, for example, <span class="tex-span">(3, 30)</span>, but none of them fits the condition <span class="tex-span"><i>l</i> ≤ <i>a</i>, <i>b</i> ≤ <i>r</i></span>.</p>
