## Description

<div><p>Eugeny has array <span class="tex-span"><i>a</i> = <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> integers. Each integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals to -1, or to 1. Also, he has <span class="tex-span"><i>m</i></span> queries:</p><ul> <li> Query number <span class="tex-span"><i>i</i></span> is given as a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. </li><li> The response to the query will be integer <span class="tex-span">1</span>, if the elements of array <span class="tex-span"><i>a</i></span> can be rearranged so as the sum <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub> + <i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub> + 1</sub> + ... + <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub> = 0</span>, otherwise the response to the query will be integer <span class="tex-span">0</span>. </li></ul><p>Help Eugeny, answer all his queries.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub> = </span>-<span class="tex-span">1, 1)</span>. Next <span class="tex-span"><i>m</i></span> lines contain Eugene's queries. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the responses to Eugene's queries in the order they occur in the input.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub> = </span>-<span class="tex-span">1, 1)</span>. Next <span class="tex-span"><i>m</i></span> lines contain Eugene's queries. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the responses to Eugene's queries in the order they occur in the input.</p>





```input1
2 3
1 -1
1 1
1 2
2 2

```




```input2
5 5
-1 1 1 1 -1
1 1
2 3
3 5
2 5
1 5

```




```output1
0
1
0

```




```output2
0
1
0
1
0

```


