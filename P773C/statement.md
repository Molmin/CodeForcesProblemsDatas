## Description

<div><p>It can be shown that any positive integer <span class="tex-span"><i>x</i></span> can be uniquely represented as <span class="tex-span"><i>x</i> = 1 + 2 + 4 + ... + 2<sup class="upper-index"><i>k</i> - 1</sup> + <i>r</i></span>, where <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>r</i></span> are integers, <span class="tex-span"><i>k</i> ≥ 0</span>, <span class="tex-span">0 &lt; <i>r</i> ≤ 2<sup class="upper-index"><i>k</i></sup></span>. Let's call that representation <span class="tex-font-style-underline">prairie partition</span> of <span class="tex-span"><i>x</i></span>.</p><p>For example, the prairie partitions of <span class="tex-span">12</span>, <span class="tex-span">17</span>, <span class="tex-span">7</span> and <span class="tex-span">1</span> are: </p><center> <span class="tex-span">12 = 1 + 2 + 4 + 5</span>,<p><span class="tex-span">17 = 1 + 2 + 4 + 8 + 2</span>,</p><p><span class="tex-span">7 = 1 + 2 + 4</span>,</p><p><span class="tex-span">1 = 1</span>. </p></center><p>Alice took a sequence of positive integers (possibly with repeating elements), replaced every element with the sequence of summands in its prairie partition, arranged the resulting numbers in non-decreasing order and gave them to Borys. Now Borys wonders how many elements Alice's original sequence could contain. Find all possible options!</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of numbers given from Alice to Borys.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>; <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>a</i><sub class="lower-index"><i>n</i></sub></span>)&nbsp;— the numbers given from Alice to Borys.</p></div><div class="output-specification"><p>Output, <span class="tex-font-style-bf">in increasing order</span>, all possible values of <span class="tex-span"><i>m</i></span> such that there exists a sequence of positive integers of length <span class="tex-span"><i>m</i></span> such that if you replace every element with the summands in its prairie partition and arrange the resulting numbers in non-decreasing order, you will get the sequence given in the input.</p><p>If there are no such values of <span class="tex-span"><i>m</i></span>, output a single integer <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of numbers given from Alice to Borys.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>; <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>a</i><sub class="lower-index"><i>n</i></sub></span>)&nbsp;— the numbers given from Alice to Borys.</p>

## Output

<p>Output, <span class="tex-font-style-bf">in increasing order</span>, all possible values of <span class="tex-span"><i>m</i></span> such that there exists a sequence of positive integers of length <span class="tex-span"><i>m</i></span> such that if you replace every element with the summands in its prairie partition and arrange the resulting numbers in non-decreasing order, you will get the sequence given in the input.</p><p>If there are no such values of <span class="tex-span"><i>m</i></span>, output a single integer <span class="tex-font-style-tt">-1</span>.</p>





```input1
8
1 1 2 2 3 4 5 8

```




```input2
6
1 1 1 2 2 2

```




```input3
5
1 2 4 4 4

```




```output1
2 

```




```output2
2 3 

```




```output3
-1

```



## Note

<p>In the first example, Alice could get the input sequence from <span class="tex-span">[6, 20]</span> as the original sequence.</p><p>In the second example, Alice's original sequence could be either <span class="tex-span">[4, 5]</span> or <span class="tex-span">[3, 3, 3]</span>.</p>
