## Description

<div><p>Ilya is very fond of graphs, especially trees. During his last trip to the forest Ilya found a very interesting tree rooted at vertex <span class="tex-span">1</span>. There is an integer number written on each vertex of the tree; the number written on vertex <span class="tex-span"><i>i</i></span> is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Ilya believes that the beauty of the vertex <span class="tex-span"><i>x</i></span> is the greatest common divisor of all numbers written on the vertices on the path from the root to <span class="tex-span"><i>x</i></span>, including this vertex itself. In addition, Ilya can change the number in one arbitrary vertex to <span class="tex-span">0</span> or leave all vertices unchanged. Now for each vertex Ilya wants to know the maximum possible beauty it can have.</p><p><span class="tex-font-style-it">For each vertex the answer must be considered independently.</span></p><p><span class="tex-font-style-it">The beauty of the root equals to number written on it.</span></p></div><div class="input-specification"><p>First line contains one integer number <span class="tex-span"><i>n</i></span>&nbsp;— the number of vertices in tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Next line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Each of next <span class="tex-span"><i>n</i> - 1</span> lines contains two integer numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i> ≠ <i>y</i></span>), which means that there is an edge <span class="tex-span">(<i>x</i>, <i>y</i>)</span> in the tree.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> numbers separated by spaces, where <span class="tex-span"><i>i</i></span>-th number equals to maximum possible beauty of vertex <span class="tex-span"><i>i</i></span>.</p></div>

## Input

<p>First line contains one integer number <span class="tex-span"><i>n</i></span>&nbsp;— the number of vertices in tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Next line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Each of next <span class="tex-span"><i>n</i> - 1</span> lines contains two integer numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i> ≠ <i>y</i></span>), which means that there is an edge <span class="tex-span">(<i>x</i>, <i>y</i>)</span> in the tree.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> numbers separated by spaces, where <span class="tex-span"><i>i</i></span>-th number equals to maximum possible beauty of vertex <span class="tex-span"><i>i</i></span>.</p>





```input1
2
6 2
1 2

```




```input2
3
6 2 3
1 2
1 3

```




```input3
1
10

```




```output1
6 6 

```




```output2
6 6 6 

```




```output3
10 

```


