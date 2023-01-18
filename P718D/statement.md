## Description

<div><p><span class="tex-font-style-it">During the chemistry lesson Andrew learned that the saturated hydrocarbons (alkanes) enter into radical chlorination reaction. Andrew is a very curious boy, so he wondered how many different products of the reaction may be forms for a given alkane. He managed to solve the task for small molecules, but for large ones he faced some difficulties and asks you to help.</span></p><p>Formally, you are given a tree consisting of <span class="tex-span"><i>n</i></span> vertices, such that the degree of each vertex doesn't exceed <span class="tex-span">4</span>. You have to count the number of distinct non-isomorphic trees that can be obtained by adding to this tree one new vertex and one new edge, such that the graph is still the tree and the degree of each vertex doesn't exceed <span class="tex-span">4</span>.</p><p>Two trees are isomorphic if there exists a bijection <span class="tex-span"><i>f</i>(<i>v</i>)</span> such that vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are connected by an edge if and only if vertices <span class="tex-span"><i>f</i>(<i>v</i>)</span> and <span class="tex-span"><i>f</i>(<i>u</i>)</span> are connected by an edge.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of vertices in the tree.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines with edges descriptions. Each edge is given by two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of vertices connected by an edge. It's guaranteed that the given graph is a tree and the degree of each vertex doesn't exceed <span class="tex-span">4</span>.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the answer to the question.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of vertices in the tree.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines with edges descriptions. Each edge is given by two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of vertices connected by an edge. It's guaranteed that the given graph is a tree and the degree of each vertex doesn't exceed <span class="tex-span">4</span>.</p>

## Output

<p>Print one integer&nbsp;— the answer to the question.</p>





```input1
4
1 2
2 3
2 4

```




```input2
5
1 2
1 3
1 4
1 5

```




```input3
5
2 5
5 3
4 3
4 1

```




```output1
2

```




```output2
1

```




```output3
3

```



## Note

<p>In the first sample, one can add new vertex to any existing vertex, but the trees we obtain by adding a new vertex to vertices <span class="tex-span">1</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span> are isomorphic, thus the answer is <span class="tex-span">2</span>.</p><p>In the second sample, one can't add new vertex to the first vertex, as its degree is already equal to four. Trees, obtained by adding a new vertex to vertices <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span> and <span class="tex-span">5</span> are isomorphic, thus the answer is <span class="tex-span">1</span>.</p>
