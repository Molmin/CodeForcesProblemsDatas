## Description

<div><p>You're given a tree with <span class="tex-span"><i>n</i></span> vertices rooted at <span class="tex-span">1</span>.</p><p>We say that there's a <span class="tex-span"><i>k</i></span>-ary heap of depth <span class="tex-span"><i>m</i></span> located at <span class="tex-span"><i>u</i></span> if the following holds:</p><ul> <li> For <span class="tex-span"><i>m</i> = 1</span> <span class="tex-span"><i>u</i></span> itself is a <span class="tex-span"><i>k</i></span>-ary heap of depth <span class="tex-span">1</span>. </li><li> For <span class="tex-span"><i>m</i> &gt; 1</span> vertex <span class="tex-span"><i>u</i></span> is a <span class="tex-span"><i>k</i></span>-ary heap of depth <span class="tex-span"><i>m</i></span> if <span class="tex-font-style-bf">at least</span> <span class="tex-span"><i>k</i></span> of its children are <span class="tex-span"><i>k</i></span>-ary heaps of depth <span class="tex-font-style-bf">at least</span> <span class="tex-span"><i>m</i> - 1</span>. </li></ul><p>Denote <span class="tex-span"><i>dp</i><sub class="lower-index"><i>k</i></sub>(<i>u</i>)</span> as maximum depth of <span class="tex-span"><i>k</i></span>-ary heap in the subtree of <span class="tex-span"><i>u</i></span> (including <span class="tex-span"><i>u</i></span>). Your goal is to compute <img align="middle" class="tex-formula" src="file://R72hRbtl.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> denoting the size of the tree <span class="tex-span">(2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>. </p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain two integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> each, describing vertices connected by <span class="tex-span"><i>i</i></span>-th edge.</p><p>It's guaranteed that the given configuration forms a tree.</p></div><div class="output-specification"><p>Output the answer to the task.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> denoting the size of the tree <span class="tex-span">(2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>. </p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain two integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> each, describing vertices connected by <span class="tex-span"><i>i</i></span>-th edge.</p><p>It's guaranteed that the given configuration forms a tree.</p>

## Output

<p>Output the answer to the task.</p>





```input1
4
1 3
2 3
4 3

```




```input2
4
1 2
2 3
3 4

```




```output1
21

```




```output2
22

```



## Note

<p>Consider sample case one.</p><p>For <span class="tex-span"><i>k</i> ≥ 3</span> all <span class="tex-span"><i>dp</i><sub class="lower-index"><i>k</i></sub></span> will be equal to <span class="tex-span">1</span>.</p><p>For <span class="tex-span"><i>k</i> = 2</span> <span class="tex-span"><i>dp</i><sub class="lower-index"><i>k</i></sub></span> is <span class="tex-span">2</span> if <img align="middle" class="tex-formula" src="file://vkhl1Amc.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span">1</span> otherwise.</p><p>For <span class="tex-span"><i>k</i> = 1</span> <span class="tex-span"><i>dp</i><sub class="lower-index"><i>k</i></sub></span> values are <span class="tex-span">(3, 1, 2, 1)</span> respectively.</p><p>To sum up, <span class="tex-span">4·1 + 4·1 + 2·2 + 2·1 + 3 + 1 + 2 + 1 = 21</span>.</p>
