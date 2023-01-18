## Description

<div><p>John Doe started thinking about graphs. After some thought he decided that he wants to paint an undirected graph, containing exactly <span class="tex-span"><i>k</i></span> cycles of length <span class="tex-span">3</span>. </p><p>A cycle of length <span class="tex-span">3</span> is an unordered group of three distinct graph vertices <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, such that each pair of them is connected by a graph edge. </p><p>John has been painting for long, but he has not been a success. Help him find such graph. Note that the number of vertices there shouldn't exceed <span class="tex-span">100</span>, or else John will have problems painting it.</p></div><div class="input-specification"><p>A single line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cycles of length <span class="tex-span">3</span> in the required graph.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — the number of vertices in the found graph. In each of next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>n</i></span> characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>": the <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>j</i></span>-th line should equal "<span class="tex-font-style-tt">0</span>", if vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> do not have an edge between them, otherwise it should equal "<span class="tex-font-style-tt">1</span>". Note that as the required graph is undirected, the <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>j</i></span>-th line must equal the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line. The graph shouldn't contain self-loops, so the <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line must equal "<span class="tex-font-style-tt">0</span>" for all <span class="tex-span"><i>i</i></span>.</p></div>

## Input

<p>A single line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cycles of length <span class="tex-span">3</span> in the required graph.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — the number of vertices in the found graph. In each of next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>n</i></span> characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>": the <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>j</i></span>-th line should equal "<span class="tex-font-style-tt">0</span>", if vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> do not have an edge between them, otherwise it should equal "<span class="tex-font-style-tt">1</span>". Note that as the required graph is undirected, the <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>j</i></span>-th line must equal the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line. The graph shouldn't contain self-loops, so the <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line must equal "<span class="tex-font-style-tt">0</span>" for all <span class="tex-span"><i>i</i></span>.</p>





```input1
1

```




```input2
10

```




```output1
3
011
101
110

```




```output2
5
01111
10111
11011
11101
11110

```


