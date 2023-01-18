## Description

<div><p>Little Petya has a birthday soon. Due this wonderful event, Petya's friends decided to give him sweets. The total number of Petya's friends equals to <span class="tex-span"><i>n</i></span>.</p><p>Let us remind you the definition of the greatest common divisor: <span class="tex-span"><i>GCD</i>(<i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub>) = <i>d</i></span>, where <span class="tex-span"><i>d</i></span> represents such a maximal positive number that each <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>) is evenly divisible by <span class="tex-span"><i>d</i></span>. At that, we assume that all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s are greater than zero.</p><p>Knowing that Petya is keen on programming, his friends has agreed beforehand that the <span class="tex-span">1</span>-st friend gives <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> sweets, the <span class="tex-span">2</span>-nd one gives <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> sweets, ..., the <span class="tex-span"><i>n</i></span>-th one gives <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> sweets. At the same time, for any <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>) they want the <span class="tex-span"><i>GCD</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>)</span> not to be equal to <span class="tex-span">1</span>. However, they also want the following condition to be satisfied: <span class="tex-span"><i>GCD</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>) = 1</span>. One more: all the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> should be distinct.</p><p>Help the friends to choose the suitable numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>).</p></div><div class="output-specification"><p>If there is no answer, print "<span class="tex-font-style-tt">-1</span>" without quotes. Otherwise print a set of <span class="tex-span"><i>n</i></span> distinct positive numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Each line must contain one number. Each number must consist of not more than <span class="tex-span">100</span> digits, and must not contain any leading zeros. If there are several solutions to that problem, print any of them.</p><p>Do not forget, please, that all of the following conditions must be true:</p><ul><li> For every <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>): <span class="tex-span"><i>GCD</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>) ≠ 1</span></li><li> <span class="tex-span"><i>GCD</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>) = 1</span></li><li> For every <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i></span>): <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub></span> </li></ul><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>).</p>

## Output

<p>If there is no answer, print "<span class="tex-font-style-tt">-1</span>" without quotes. Otherwise print a set of <span class="tex-span"><i>n</i></span> distinct positive numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Each line must contain one number. Each number must consist of not more than <span class="tex-span">100</span> digits, and must not contain any leading zeros. If there are several solutions to that problem, print any of them.</p><p>Do not forget, please, that all of the following conditions must be true:</p><ul><li> For every <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>): <span class="tex-span"><i>GCD</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>) ≠ 1</span></li><li> <span class="tex-span"><i>GCD</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>) = 1</span></li><li> For every <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i></span>): <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub></span> </li></ul><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
3

```




```input2
4

```




```output1
99
55
11115

```




```output2
385
360
792
8360

```


