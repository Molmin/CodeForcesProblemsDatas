## Description

<div><p>Arpa has found a list containing <span class="tex-span"><i>n</i></span> numbers. He calls a list bad if and only if it is not empty and <span class="tex-font-style-tt">gcd</span> (see notes section for more information) of numbers in the list is <span class="tex-span">1</span>.</p><p>Arpa can perform two types of operations:</p><ul> <li> Choose a number and delete it with cost <span class="tex-span"><i>x</i></span>. </li><li> Choose a number and increase it by <span class="tex-span">1</span> with cost <span class="tex-span"><i>y</i></span>. </li></ul><p>Arpa can apply these operations to as many numbers as he wishes, and he is allowed to apply the second operation arbitrarily many times on the same number.</p><p>Help Arpa to find the minimum possible cost to make the list good.</p></div><div class="input-specification"><p>First line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of elements in the list and the integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the elements of the list.</p></div><div class="output-specification"><p>Print a single integer: the minimum possible cost to make the list good.</p></div>

## Input

<p>First line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of elements in the list and the integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the elements of the list.</p>

## Output

<p>Print a single integer: the minimum possible cost to make the list good.</p>





```input1
4 23 17
1 17 17 16

```




```input2
10 6 2
100 49 71 73 66 96 8 60 41 63

```




```output1
40

```




```output2
10

```



## Note

<p>In example, number <span class="tex-span">1</span> must be deleted (with cost <span class="tex-span">23</span>) and number <span class="tex-span">16</span> must increased by <span class="tex-span">1</span> (with cost <span class="tex-span">17</span>).</p><p>A <span class="tex-font-style-tt">gcd</span> (greatest common divisor) of a set of numbers is the maximum integer that divides all integers in the set. Read more about gcd <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">here</a>.</p>
