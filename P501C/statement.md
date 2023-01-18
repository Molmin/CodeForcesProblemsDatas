## Description

<div><p>Let's define a forest as a non-directed acyclic graph (also without loops and parallel edges). One day Misha played with the forest consisting of <span class="tex-span"><i>n</i></span> vertices. For each vertex <span class="tex-span"><i>v</i></span> from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span> he wrote down two integers, <span class="tex-span"><i>degree</i><sub class="lower-index"><i>v</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>v</i></sub></span>, were the first integer is the number of vertices adjacent to vertex <span class="tex-span"><i>v</i></span>, and the second integer is the XOR sum of the numbers of vertices adjacent to <span class="tex-span"><i>v</i></span> (if there were no adjacent vertices, he wrote down <span class="tex-span">0</span>). </p><p>Next day Misha couldn't remember what graph he initially had. Misha has values <span class="tex-span"><i>degree</i><sub class="lower-index"><i>v</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>v</i></sub></span> left, though. Help him find the number of edges and the edges of the initial graph. It is guaranteed that there exists a forest that corresponds to the numbers written by Misha.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2<sup class="upper-index">16</sup></span>), the number of vertices in the graph.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next lines contains numbers <span class="tex-span"><i>degree</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>degree</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">16</sup></span>), separated by a space.</p></div><div class="output-specification"><p>In the first line print number <span class="tex-span"><i>m</i></span>, the number of edges of the graph.</p><p>Next print <span class="tex-span"><i>m</i></span> lines, each containing two distinct numbers, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ <i>n</i> - 1</span>), corresponding to edge <span class="tex-span">(<i>a</i>, <i>b</i>)</span>.</p><p>Edges can be printed in any order; vertices of the edge can also be printed in any order.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2<sup class="upper-index">16</sup></span>), the number of vertices in the graph.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next lines contains numbers <span class="tex-span"><i>degree</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>degree</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">16</sup></span>), separated by a space.</p>

## Output

<p>In the first line print number <span class="tex-span"><i>m</i></span>, the number of edges of the graph.</p><p>Next print <span class="tex-span"><i>m</i></span> lines, each containing two distinct numbers, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ <i>n</i> - 1</span>), corresponding to edge <span class="tex-span">(<i>a</i>, <i>b</i>)</span>.</p><p>Edges can be printed in any order; vertices of the edge can also be printed in any order.</p>





```input1
3
2 3
1 0
1 0

```




```input2
2
1 1
1 0

```




```output1
2
1 0
2 0

```




```output2
1
0 1

```



## Note

<p>The XOR sum of numbers is the result of bitwise adding numbers modulo <span class="tex-span">2</span>. This operation exists in many modern programming languages. For example, in languages C++, Java and Python it is represented as "<span class="tex-font-style-tt">^</span>", and in Pascal — as "xor".</p>
