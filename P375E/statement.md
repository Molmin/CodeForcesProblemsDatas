## Description

<div><p>You have a weighted tree, consisting of <span class="tex-span"><i>n</i></span> vertices. Each vertex is either painted black or is painted red. A red and black tree is called <span class="tex-font-style-it">beautiful</span>, if for any its vertex we can find a black vertex at distance at most <span class="tex-span"><i>x</i></span>.</p><p>The distance between two nodes is the shortest path between them.</p><p>You have a red and black tree. Your task is to make it beautiful in the minimum number of color swap operations. In one color swap operation, you can choose two vertices of different colors and paint each of them the other color. In other words, if you choose a red vertex <span class="tex-span"><i>p</i></span> and a black vertex <span class="tex-span"><i>q</i></span>, then in one operation you are allowed to paint <span class="tex-span"><i>p</i></span> black and paint <span class="tex-span"><i>q</i></span> red.</p><p>Print the minimum number of required actions.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 500;&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers, each of them is either a zero or one. If the <span class="tex-span"><i>i</i></span>-th number equals 1, then vertex <span class="tex-span"><i>i</i></span> of the tree is black, otherwise vertex <span class="tex-span"><i>i</i></span> is red. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the tree edges. The <span class="tex-span"><i>j</i></span>-th line contains integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub>&nbsp;<i>v</i><sub class="lower-index"><i>j</i></sub>&nbsp;<i>w</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>j</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub>;&nbsp;1 ≤ <i>w</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> which means that the tree has an edge of weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> between vertices <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Assume that the tree vertices are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of required swap operations.</p><p>If it is impossible to get a beautiful tree at any number of operations, print -1.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 500;&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers, each of them is either a zero or one. If the <span class="tex-span"><i>i</i></span>-th number equals 1, then vertex <span class="tex-span"><i>i</i></span> of the tree is black, otherwise vertex <span class="tex-span"><i>i</i></span> is red. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the tree edges. The <span class="tex-span"><i>j</i></span>-th line contains integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub>&nbsp;<i>v</i><sub class="lower-index"><i>j</i></sub>&nbsp;<i>w</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>j</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub>;&nbsp;1 ≤ <i>w</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> which means that the tree has an edge of weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> between vertices <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Assume that the tree vertices are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print a single integer — the minimum number of required swap operations.</p><p>If it is impossible to get a beautiful tree at any number of operations, print -1.</p>





```input1
3 2
1 0 0
1 2 2
2 3 2

```




```input2
4 2
0 1 0 0
1 2 2
2 3 2
3 4 2

```




```output1
1

```




```output2
-1

```


