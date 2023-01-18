## Description

<div><p>Appleman has a tree with <span class="tex-span"><i>n</i></span> vertices. Some of the vertices (at least one) are colored black and other vertices are colored white.</p><p>Consider a set consisting of <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> &lt; <i>n</i>)</span> edges of Appleman's tree. If Appleman deletes these edges from the tree, then it will split into <span class="tex-span">(<i>k</i> + 1)</span> parts. Note, that each part will be a tree with colored vertices.</p><p>Now Appleman wonders, what is the number of sets splitting the tree in such a way that each resulting part will have exactly one black vertex? Find this number modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2  ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tree vertices. </p><p>The second line contains the description of the tree: <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">0</sub>, <i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i> - 2</sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>). Where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that there is an edge connecting vertex <span class="tex-span">(<i>i</i> + 1)</span> of the tree and vertex <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Consider tree vertices are numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>.</p><p>The third line contains the description of the colors of the vertices: <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is either <span class="tex-span">0</span> or <span class="tex-span">1</span>). If <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span">1</span>, vertex <span class="tex-span"><i>i</i></span> is colored black. Otherwise, vertex <span class="tex-span"><i>i</i></span> is colored white.</p></div><div class="output-specification"><p>Output a single integer — the number of ways to split the tree modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2  ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tree vertices. </p><p>The second line contains the description of the tree: <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">0</sub>, <i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i> - 2</sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>). Where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that there is an edge connecting vertex <span class="tex-span">(<i>i</i> + 1)</span> of the tree and vertex <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Consider tree vertices are numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>.</p><p>The third line contains the description of the colors of the vertices: <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is either <span class="tex-span">0</span> or <span class="tex-span">1</span>). If <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span">1</span>, vertex <span class="tex-span"><i>i</i></span> is colored black. Otherwise, vertex <span class="tex-span"><i>i</i></span> is colored white.</p>

## Output

<p>Output a single integer — the number of ways to split the tree modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
3
0 0
0 1 1

```




```input2
6
0 1 1 0 4
1 1 0 0 1 0

```




```input3
10
0 1 2 1 4 4 4 0 8
0 0 0 1 0 1 1 0 0 1

```




```output1
2

```




```output2
1

```




```output3
27

```


