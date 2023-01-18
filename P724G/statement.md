## Description

<div><p>You are given an undirected graph, constisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. Each edge of the graph has some non-negative integer written on it.</p><p>Let's call a triple <span class="tex-span">(<i>u</i>, <i>v</i>, <i>s</i>)</span> <span class="tex-font-style-bf">interesting</span>, if <span class="tex-span">1 ≤ <i>u</i> &lt; <i>v</i> ≤ <i>n</i></span> and there is a path (<span class="tex-font-style-bf">possibly non-simple</span>, i.e. it can visit the same vertices and edges multiple times) between vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> such that xor of all numbers written on the edges of this path is equal to <span class="tex-span"><i>s</i></span>. <span class="tex-font-style-bf">When we compute the value s for some path, each edge is counted in xor as many times, as it appear on this path.</span> It's not hard to prove that there are finite number of such triples.</p><p>Calculate the sum over modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> of the values of <span class="tex-span"><i>s</i></span> over all <span class="tex-font-style-bf">interesting</span> triples.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and&nbsp;<span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— numbers of vertices and edges in the given graph.</p><p>The follow <span class="tex-span"><i>m</i></span> lines contain three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and&nbsp;<span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— vertices connected by the edge and integer written on it. It is guaranteed that graph doesn't contain self-loops and multiple edges.</p></div><div class="output-specification"><p>Print the single integer, equal to the described sum over modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and&nbsp;<span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— numbers of vertices and edges in the given graph.</p><p>The follow <span class="tex-span"><i>m</i></span> lines contain three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and&nbsp;<span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— vertices connected by the edge and integer written on it. It is guaranteed that graph doesn't contain self-loops and multiple edges.</p>

## Output

<p>Print the single integer, equal to the described sum over modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4 4
1 2 1
1 3 2
2 3 3
3 4 1

```




```input2
4 4
1 2 1
2 3 2
3 4 4
4 1 8

```




```input3
8 6
1 2 2
2 3 1
2 4 4
4 5 5
4 6 3
7 8 5

```




```output1
12

```




```output2
90

```




```output3
62

```



## Note

<p>In the first example the are <span class="tex-span">6</span> interesting triples: </p><ol> <li> <span class="tex-span">(1, 2, 1)</span> </li><li> <span class="tex-span">(1, 3, 2)</span> </li><li> <span class="tex-span">(1, 4, 3)</span> </li><li> <span class="tex-span">(2, 3, 3)</span> </li><li> <span class="tex-span">(2, 4, 2)</span> </li><li> <span class="tex-span">(3, 4, 1)</span> </li></ol> The sum is equal to <span class="tex-span">1 + 2 + 3 + 3 + 2 + 1 = 12</span>.<p>In the second example the are <span class="tex-span">12</span> interesting triples: </p><ol> <li> <span class="tex-span">(1, 2, 1)</span> </li><li> <span class="tex-span">(2, 3, 2)</span> </li><li> <span class="tex-span">(1, 3, 3)</span> </li><li> <span class="tex-span">(3, 4, 4)</span> </li><li> <span class="tex-span">(2, 4, 6)</span> </li><li> <span class="tex-span">(1, 4, 7)</span> </li><li> <span class="tex-span">(1, 4, 8)</span> </li><li> <span class="tex-span">(2, 4, 9)</span> </li><li> <span class="tex-span">(3, 4, 11)</span> </li><li> <span class="tex-span">(1, 3, 12)</span> </li><li> <span class="tex-span">(2, 3, 13)</span> </li><li> <span class="tex-span">(1, 2, 14)</span> </li></ol> The sum is equal to <span class="tex-span">1 + 2 + 3 + 4 + 6 + 7 + 8 + 9 + 11 + 12 + 13 + 14 = 90</span>.
