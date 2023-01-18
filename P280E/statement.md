## Description

<div><p>You've got a non-decreasing sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>x</i><sub class="lower-index"><i>n</i></sub> ≤ <i>q</i>)</span>. You've also got two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>a</i> ≤ <i>b</i>;&nbsp;<i>a</i>·(<i>n</i> - 1) &lt; <i>q</i>)</span>.</p><p>Your task is to transform sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> into some sequence <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>q</i>;&nbsp;<i>a</i> ≤ <i>y</i><sub class="lower-index"><i>i</i> + 1</sub> - <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i>)</span>. The transformation price is the following sum: <img align="middle" class="tex-formula" src="file://oZuSZ2NJ.png" style="max-width: 100.0%;max-height: 100.0%;">. Your task is to choose such sequence <span class="tex-span"><i>y</i></span> that minimizes the described transformation price.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i>, <i>q</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 6000;&nbsp;1 ≤ <i>q</i>, <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>a</i>·(<i>n</i> - 1) &lt; <i>q</i>;&nbsp;<i>a</i> ≤ <i>b</i>)</span>.</p><p>The second line contains a non-decreasing integer sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>x</i><sub class="lower-index"><i>n</i></sub> ≤ <i>q</i>)</span>.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>n</i></span> real numbers — the sought sequence <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>q</i>;&nbsp;<i>a</i> ≤ <i>y</i><sub class="lower-index"><i>i</i> + 1</sub> - <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i>)</span>. In the second line print the minimum transformation price, that is, <img align="middle" class="tex-formula" src="file://4u7BSoXe.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>If there are multiple optimal answers you can print any of them.</p><p>The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i>, <i>q</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 6000;&nbsp;1 ≤ <i>q</i>, <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>a</i>·(<i>n</i> - 1) &lt; <i>q</i>;&nbsp;<i>a</i> ≤ <i>b</i>)</span>.</p><p>The second line contains a non-decreasing integer sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>x</i><sub class="lower-index"><i>n</i></sub> ≤ <i>q</i>)</span>.</p>

## Output

<p>In the first line print <span class="tex-span"><i>n</i></span> real numbers — the sought sequence <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>q</i>;&nbsp;<i>a</i> ≤ <i>y</i><sub class="lower-index"><i>i</i> + 1</sub> - <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i>)</span>. In the second line print the minimum transformation price, that is, <img align="middle" class="tex-formula" src="file://4u7BSoXe.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>If there are multiple optimal answers you can print any of them.</p><p>The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3 6 2 2
1 4 6

```




```input2
10 100000 8714 9344
3378 14705 17588 22672 32405 34309 37446 51327 81228 94982

```




```output1
1.666667 3.666667 5.666667 
0.666667

```




```output2
1.000000 8715.000000 17429.000000 26143.000000 34857.000000 43571.000000 52285.000000 61629.000000 70973.000000 80317.000000 
797708674.000000

```


