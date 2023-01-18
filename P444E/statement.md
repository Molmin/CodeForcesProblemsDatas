## Description

<div><p><span class="tex-font-style-it">DZY loves planting, and he enjoys solving tree problems.</span></p><p>DZY has a weighted tree (connected undirected graph without cycles) containing <span class="tex-span"><i>n</i></span> nodes (they are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>). He defines the function <span class="tex-span"><i>g</i>(<i>x</i>, <i>y</i>)</span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span> as the longest edge in the shortest path between nodes <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. Specially <span class="tex-span"><i>g</i>(<i>z</i>, <i>z</i>) = 0</span> for every <span class="tex-span"><i>z</i></span>.</p><p>For every integer sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, DZY defines <span class="tex-span"><i>f</i>(<i>p</i>)</span> as <img align="middle" class="tex-formula" src="file://yMyXSNVH.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>DZY wants to find such a sequence <span class="tex-span"><i>p</i></span> that <span class="tex-span"><i>f</i>(<i>p</i>)</span> has maximum possible value. But there is one more restriction: the element <span class="tex-span"><i>j</i></span> can appear in <span class="tex-span"><i>p</i></span> at most <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> times.</p><p>Please, find the maximum possible <span class="tex-span"><i>f</i>(<i>p</i>)</span> under the described restrictions.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 3000)</span>.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10000)</span>, denoting an edge between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with length <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that these edges form a tree.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines describes an element of sequence <span class="tex-span"><i>x</i></span>. The <span class="tex-span"><i>j</i></span>-th line contains an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub>&nbsp;(1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print a single integer representing the answer.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 3000)</span>.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10000)</span>, denoting an edge between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with length <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that these edges form a tree.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines describes an element of sequence <span class="tex-span"><i>x</i></span>. The <span class="tex-span"><i>j</i></span>-th line contains an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub>&nbsp;(1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Print a single integer representing the answer.</p>





```input1
4
1 2 1
2 3 2
3 4 3
1
1
1
1

```




```input2
4
1 2 1
2 3 2
3 4 3
4
4
4
4

```




```output1
2

```




```output2
3

```



## Note

<p>In the first sample, one of the optimal <span class="tex-span"><i>p</i></span> is <span class="tex-span">[4, 3, 2, 1]</span>.</p>
