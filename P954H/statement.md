## Description

<div><p>You are given a rooted tree. Let's denote <span class="tex-span"><i>d</i>(<i>x</i>)</span> as depth of node <span class="tex-span"><i>x</i></span>: depth of the root is <span class="tex-span">1</span>, depth of any other node <span class="tex-span"><i>x</i></span> is <span class="tex-span"><i>d</i>(<i>y</i>) + 1</span>, where <span class="tex-span"><i>y</i></span> is a parent of <span class="tex-span"><i>x</i></span>.</p><p>The tree has the following property: every node <span class="tex-span"><i>x</i></span> with <span class="tex-span"><i>d</i>(<i>x</i>) = <i>i</i></span> has exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> children. Maximum possible depth of a node is <span class="tex-span"><i>n</i></span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = 0</span>.</p><p>We define <span class="tex-span"><i>f</i><sub class="lower-index"><i>k</i></sub></span> as the number of unordered pairs of vertices in the tree such that the number of edges on the simple path between them is equal to <span class="tex-span"><i>k</i></span>.</p><p>Calculate <span class="tex-span"><i>f</i><sub class="lower-index"><i>k</i></sub></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> for every <span class="tex-span">1 ≤ <i>k</i> ≤ 2<i>n</i> - 2</span>.</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2  ≤  <i>n</i>  ≤  5 000</span>) — the maximum depth of a node.</p><p>The second line of input contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">2 ≤  <i>a</i><sub class="lower-index"><i>i</i></sub>  ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of children of every node <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>d</i>(<i>x</i>) = <i>i</i></span>. Since <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = 0</span>, it is not given in the input.</p></div><div class="output-specification"><p>Print <span class="tex-span">2<i>n</i> - 2</span> numbers. The <span class="tex-span"><i>k</i></span>-th of these numbers must be equal to <span class="tex-span"><i>f</i><sub class="lower-index"><i>k</i></sub></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2  ≤  <i>n</i>  ≤  5 000</span>) — the maximum depth of a node.</p><p>The second line of input contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">2 ≤  <i>a</i><sub class="lower-index"><i>i</i></sub>  ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of children of every node <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>d</i>(<i>x</i>) = <i>i</i></span>. Since <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = 0</span>, it is not given in the input.</p>

## Output

<p>Print <span class="tex-span">2<i>n</i> - 2</span> numbers. The <span class="tex-span"><i>k</i></span>-th of these numbers must be equal to <span class="tex-span"><i>f</i><sub class="lower-index"><i>k</i></sub></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4
2 2 2

```




```input2
3
2 3

```




```output1
14 19 20 20 16 16
```




```output2
8 13 6 9
```



## Note

<p>This the tree from the first sample: </p><center> <img class="tex-graphics" src="file://s0xIGDho.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
