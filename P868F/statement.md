## Description

<div><p>You are given an array of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span>. The cost of a subsegment is the number of unordered pairs of distinct indices within the subsegment that contain equal elements. Split the given array into <span class="tex-span"><i>k</i></span> non-intersecting non-empty subsegments so that the sum of their costs is minimum possible. Each element should be present in exactly one subsegment.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>min</i> (<i>n</i>, 20))</span> &nbsp;— the length of the array and the number of segments you need to split the array into.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>Print single integer: the minimum possible total cost of resulting subsegments.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>min</i> (<i>n</i>, 20))</span> &nbsp;— the length of the array and the number of segments you need to split the array into.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the elements of the array.</p>

## Output

<p>Print single integer: the minimum possible total cost of resulting subsegments.</p>





```input1
7 3
1 1 3 3 3 2 1

```




```input2
10 2
1 2 1 2 1 2 1 2 1 2

```




```input3
13 3
1 2 2 2 1 2 1 1 1 2 2 1 1

```




```output1
1

```




```output2
8

```




```output3
9

```



## Note

<p>In the first example it's optimal to split the sequence into the following three subsegments: <span class="tex-span">[1]</span>, <span class="tex-span">[1, 3]</span>, <span class="tex-span">[3, 3, 2, 1]</span>. The costs are <span class="tex-span">0</span>, <span class="tex-span">0</span> and <span class="tex-span">1</span>, thus the answer is <span class="tex-span">1</span>.</p><p>In the second example it's optimal to split the sequence in two equal halves. The cost for each half is <span class="tex-span">4</span>.</p><p>In the third example it's optimal to split the sequence in the following way: <span class="tex-span">[1, 2, 2, 2, 1]</span>, <span class="tex-span">[2, 1, 1, 1, 2]</span>, <span class="tex-span">[2, 1, 1]</span>. The costs are <span class="tex-span">4</span>, <span class="tex-span">4</span>, <span class="tex-span">1</span>.</p>
