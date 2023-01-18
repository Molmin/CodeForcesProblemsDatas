## Description

<div><p>Consider the function <span class="tex-span"><i>p</i>(<i>x</i>)</span>, where <span class="tex-span"><i>x</i></span> is an array of <span class="tex-span"><i>m</i></span> integers, which returns an array <span class="tex-span"><i>y</i></span> consisting of <span class="tex-span"><i>m</i> + 1</span> integers such that <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is equal to the sum of first <span class="tex-span"><i>i</i></span> elements of array <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>i</i> ≤ <i>m</i></span>).</p><p>You have an infinite sequence of arrays <span class="tex-span"><i>A</i><sup class="upper-index">0</sup>, <i>A</i><sup class="upper-index">1</sup>, <i>A</i><sup class="upper-index">2</sup>...</span>, where <span class="tex-span"><i>A</i><sup class="upper-index">0</sup></span> is given in the input, and for each <span class="tex-span"><i>i</i> ≥ 1</span> <span class="tex-span"><i>A</i><sup class="upper-index"><i>i</i></sup> = <i>p</i>(<i>A</i><sup class="upper-index"><i>i</i> - 1</sup>)</span>. Also you have a positive integer <span class="tex-span"><i>k</i></span>. You have to find minimum possible <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>A</i><sup class="upper-index"><i>i</i></sup></span> contains a number which is larger or equal than <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>). <span class="tex-span"><i>n</i></span> is the size of array <span class="tex-span"><i>A</i><sup class="upper-index">0</sup></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>A</i><sup class="upper-index">0</sup><sub class="lower-index">0</sub>, <i>A</i><sup class="upper-index">0</sup><sub class="lower-index">1</sub>... <i>A</i><sup class="upper-index">0</sup><sub class="lower-index"><i>n</i> - 1</sub></span> — the elements of <span class="tex-span"><i>A</i><sup class="upper-index">0</sup></span> (<span class="tex-span">0 ≤ <i>A</i><sup class="upper-index">0</sup><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). At least two elements of <span class="tex-span"><i>A</i><sup class="upper-index">0</sup></span> are positive.</p></div><div class="output-specification"><p>Print the minimum <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>A</i><sup class="upper-index"><i>i</i></sup></span> contains a number which is larger or equal than <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>). <span class="tex-span"><i>n</i></span> is the size of array <span class="tex-span"><i>A</i><sup class="upper-index">0</sup></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>A</i><sup class="upper-index">0</sup><sub class="lower-index">0</sub>, <i>A</i><sup class="upper-index">0</sup><sub class="lower-index">1</sub>... <i>A</i><sup class="upper-index">0</sup><sub class="lower-index"><i>n</i> - 1</sub></span> — the elements of <span class="tex-span"><i>A</i><sup class="upper-index">0</sup></span> (<span class="tex-span">0 ≤ <i>A</i><sup class="upper-index">0</sup><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). At least two elements of <span class="tex-span"><i>A</i><sup class="upper-index">0</sup></span> are positive.</p>

## Output

<p>Print the minimum <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>A</i><sup class="upper-index"><i>i</i></sup></span> contains a number which is larger or equal than <span class="tex-span"><i>k</i></span>.</p>





```input1
2 2
1 1

```




```input2
3 6
1 1 1

```




```input3
3 1
1 0 1

```




```output1
1

```




```output2
2

```




```output3
0

```


