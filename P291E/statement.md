## Description

<div><p>A <span class="tex-font-style-it">rooted tree</span> is a non-directed connected graph without any cycles with a distinguished vertex, which is called the tree root. Consider the vertices of a rooted tree, that consists of <span class="tex-span"><i>n</i></span> vertices, numbered from 1 to <span class="tex-span"><i>n</i></span>. In this problem the tree root is the vertex number 1.</p><p>Let's represent the length of the shortest by the number of edges path in the tree between vertices <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> as <span class="tex-span"><i>d</i>(<i>v</i>, <i>u</i>)</span>.</p><p>A <span class="tex-font-style-it">parent</span> of vertex <span class="tex-span"><i>v</i></span> in the rooted tree with the root in vertex <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>v</i> ≠ <i>r</i>)</span> is vertex <span class="tex-span"><i>p</i><sub class="lower-index"><i>v</i></sub></span>, such that <span class="tex-span"><i>d</i>(<i>r</i>, <i>p</i><sub class="lower-index"><i>v</i></sub>) + 1 = <i>d</i>(<i>r</i>, <i>v</i>)</span> and <span class="tex-font-style-bf"><span class="tex-span"><i>d</i>(<i>p</i><sub class="lower-index"><i>v</i></sub>, <i>v</i>) = 1</span></span>. For example, on the picture the parent of vertex <span class="tex-span"><i>v</i> = 5</span> is vertex <span class="tex-span"><i>p</i><sub class="lower-index">5</sub> = 2</span>.</p><p>One day Polycarpus came across a rooted tree, consisting of <span class="tex-span"><i>n</i></span> vertices. The tree wasn't exactly ordinary: it had strings written on its edges. Polycarpus positioned the tree on the plane so as to make all edges lead from top to bottom if you go from the vertex parent to the vertex (see the picture). For any edge that lead from vertex <span class="tex-span"><i>p</i><sub class="lower-index"><i>v</i></sub></span> to vertex <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 &lt; <i>v</i> ≤ <i>n</i>)</span>, he knows string <span class="tex-span"><i>s</i><sub class="lower-index"><i>v</i></sub></span> that is written on it. All strings are written on the edges from top to bottom. For example, on the picture <span class="tex-span"><i>s</i><sub class="lower-index">7</sub></span>="<span class="tex-font-style-tt">ba</span>". The characters in the strings are numbered starting from 0.</p><center> <img class="tex-graphics" src="file://UoGdd2ii.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-script">An example of Polycarpus's tree (corresponds to the example from the statement)</span> </center><p>Polycarpus defines the <span class="tex-font-style-it">position</span> in this tree as a specific letter on a specific string. The position is written as a pair of integers <span class="tex-span">(<i>v</i>, <i>x</i>)</span> that means that the position is the <span class="tex-span"><i>x</i></span>-th letter of the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>v</i></sub></span> (<span class="tex-span">1 &lt; <i>v</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> &lt; |<i>s</i><sub class="lower-index"><i>v</i></sub>|</span>), where <span class="tex-span">|<i>s</i><sub class="lower-index"><i>v</i></sub>|</span> is the length of string <span class="tex-span"><i>s</i><sub class="lower-index"><i>v</i></sub></span>. For example, the highlighted letters are positions (<span class="tex-span">2, 1</span>) and (<span class="tex-span">3, 1</span>).</p><p>Let's consider the pair of positions <span class="tex-span">(<i>v</i>, <i>x</i>)</span> and <span class="tex-span">(<i>u</i>, <i>y</i>)</span> in Polycarpus' tree, such that the way from the first position to the second goes down on each step. We will consider that the pair of such positions defines string <span class="tex-span"><i>z</i></span>. String <span class="tex-span"><i>z</i></span> consists of all letters on the way from <span class="tex-span">(<i>v</i>, <i>x</i>)</span> to <span class="tex-span">(<i>u</i>, <i>y</i>)</span>, written in the order of this path. For example, in the picture the highlighted positions define string "<span class="tex-font-style-tt">bacaba</span>".</p><p>Polycarpus has a string <span class="tex-span"><i>t</i></span>, he wants to know the number of pairs of positions that define string <span class="tex-span"><i>t</i></span>. Note that the way from the first position to the second in the pair must go down everywhere. Help him with this challenging tree-string problem!</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of vertices of Polycarpus's tree. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the tree edges. The <span class="tex-span"><i>i</i></span>-th of them contains number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> and string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i> + 1</sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i> + 1</sub> ≤ <i>n</i>;&nbsp;<i>p</i><sub class="lower-index"><i>i</i> + 1</sub> ≠ (<i>i</i> + 1))</span>. String <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i> + 1</sub></span> is non-empty and consists of lowercase English letters. The last line contains string <span class="tex-span"><i>t</i></span>. String <span class="tex-span"><i>t</i></span> consists of lowercase English letters, its length is at least 2.</p><p>It is guaranteed that the input contains at most <span class="tex-span">3·10<sup class="upper-index">5</sup></span> English letters.</p></div><div class="output-specification"><p>Print a single integer — the required number.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of vertices of Polycarpus's tree. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the tree edges. The <span class="tex-span"><i>i</i></span>-th of them contains number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> and string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i> + 1</sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i> + 1</sub> ≤ <i>n</i>;&nbsp;<i>p</i><sub class="lower-index"><i>i</i> + 1</sub> ≠ (<i>i</i> + 1))</span>. String <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i> + 1</sub></span> is non-empty and consists of lowercase English letters. The last line contains string <span class="tex-span"><i>t</i></span>. String <span class="tex-span"><i>t</i></span> consists of lowercase English letters, its length is at least 2.</p><p>It is guaranteed that the input contains at most <span class="tex-span">3·10<sup class="upper-index">5</sup></span> English letters.</p>

## Output

<p>Print a single integer — the required number.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
7
1 ab
5 bacaba
1 abacaba
2 aca
5 ba
2 ba
aba

```




```input2
7
1 ab
5 bacaba
1 abacaba
2 aca
5 ba
2 ba
bacaba

```




```output1
6

```




```output2
4

```



## Note

<p>In the first test case string "<span class="tex-font-style-tt">aba</span>" is determined by the pairs of positions: (2, 0) and (5, 0); (5, 2) and (6, 1); (5, 2) and (3, 1); (4, 0) and (4, 2); (4, 4) and (4, 6); (3, 3) and (3, 5).</p><p>Note that the string is not defined by the pair of positions (7, 1) and (5, 0), as the way between them doesn't always go down.</p>
