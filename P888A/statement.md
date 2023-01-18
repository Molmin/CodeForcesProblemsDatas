## Description

<div><p>You are given an array <span class="tex-span"><i>a</i></span>. Some element of this array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is a <span class="tex-font-style-it">local minimum</span> iff it is strictly less than both of its neighbours (that is, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>). Also the element can be called <span class="tex-font-style-it">local maximum</span> iff it is strictly greater than its neighbours (that is, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>). Since <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> have only one neighbour each, they are neither local minima nor local maxima.</p><p>An element is called a <span class="tex-font-style-it">local extremum</span> iff it is either local maximum or local minimum. Your task is to calculate the number of local extrema in the given array.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of elements in array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the elements of array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print the number of local extrema in the given array.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of elements in array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the elements of array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print the number of local extrema in the given array.</p>





```input1
3
1 2 3

```




```input2
4
1 5 2 5

```




```output1
0

```




```output2
2

```


