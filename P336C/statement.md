## Description

<div><p>Vasily the bear has got a sequence of positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Vasily the Bear wants to write out several numbers on a piece of paper so that the beauty of the numbers he wrote out was maximum. </p><p>The <span class="tex-font-style-it">beauty</span> of the written out numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> is such maximum non-negative integer <span class="tex-span"><i>v</i></span>, that number <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>and</i></span> <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>and</i></span> <span class="tex-span">...</span> <span class="tex-span"><i>and</i></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span> is divisible by number <span class="tex-span">2<sup class="upper-index"><i>v</i></sup></span> without a remainder. If such number <span class="tex-span"><i>v</i></span> doesn't exist (that is, for any non-negative integer <span class="tex-span"><i>v</i></span>, number <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>and</i></span> <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>and</i></span> <span class="tex-span">...</span> <span class="tex-span"><i>and</i></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span> is divisible by <span class="tex-span">2<sup class="upper-index"><i>v</i></sup></span> without a remainder), the beauty of the written out numbers equals -1. </p><p>Tell the bear which numbers he should write out so that the beauty of the written out numbers is maximum. If there are multiple ways to write out the numbers, you need to choose the one where the bear writes out as many numbers as possible.</p><p>Here expression <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>and</i></span> <span class="tex-span"><i>y</i></span> means applying the bitwise AND operation to numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. In programming languages C++ and Java this operation is represented by "&amp;", in Pascal — by "and".</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &gt; 0)</span>, showing how many numbers to write out. In the second line print <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> — the numbers to write out. You are allowed to print numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> in any order, but all of them must be distinct. If there are multiple ways to write out the numbers, choose the one with the maximum number of numbers to write out. If there still are multiple ways, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &gt; 0)</span>, showing how many numbers to write out. In the second line print <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> — the numbers to write out. You are allowed to print numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> in any order, but all of them must be distinct. If there are multiple ways to write out the numbers, choose the one with the maximum number of numbers to write out. If there still are multiple ways, you are allowed to print any of them.</p>





```input1
5
1 2 3 4 5

```




```input2
3
1 2 4

```




```output1
2
4 5

```




```output2
1
4

```


