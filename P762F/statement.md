## Description

<div><p>You are given two trees (connected undirected acyclic graphs) <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>.</p><p>Count the number of subtrees (connected subgraphs) of <span class="tex-span"><i>S</i></span> that are isomorphic to tree <span class="tex-span"><i>T</i></span>. Since this number can get quite large, output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Two subtrees of tree <span class="tex-span"><i>S</i></span> are considered different, if there exists a vertex in <span class="tex-span"><i>S</i></span> that belongs to exactly one of them.</p><p>Tree <span class="tex-span"><i>G</i></span> is called isomorphic to tree <span class="tex-span"><i>H</i></span> if there exists a bijection <span class="tex-span"><i>f</i></span> from the set of vertices of <span class="tex-span"><i>G</i></span> to the set of vertices of <span class="tex-span"><i>H</i></span> that has the following property: if there is an edge between vertices <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> in tree <span class="tex-span"><i>G</i></span>, then there must be an edge between vertices <span class="tex-span"><i>f</i>(<i>A</i>)</span> and <span class="tex-span"><i>f</i>(<i>B</i>)</span> in tree <span class="tex-span"><i>H</i></span>. And vice versa&nbsp;— if there is an edge between vertices <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> in tree <span class="tex-span"><i>H</i></span>, there must be an edge between <span class="tex-span"><i>f</i><sup class="upper-index"> - 1</sup>(<i>A</i>)</span> and <span class="tex-span"><i>f</i><sup class="upper-index"> - 1</sup>(<i>B</i>)</span> in tree <span class="tex-span"><i>G</i></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span">|<i>S</i>|</span> (<span class="tex-span">1 ≤ |<i>S</i>| ≤ 1000</span>) — the number of vertices of tree <span class="tex-span"><i>S</i></span>.</p><p>Next <span class="tex-span">|<i>S</i>| - 1</span> lines contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>S</i>|</span>) and describe edges of tree <span class="tex-span"><i>S</i></span>.</p><p>The next line contains a single integer <span class="tex-span">|<i>T</i>|</span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ 12</span>) — the number of vertices of tree <span class="tex-span"><i>T</i></span>.</p><p>Next <span class="tex-span">|<i>T</i>| - 1</span> lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>T</i>|</span>) and describe edges of tree <span class="tex-span"><i>T</i></span>.</p></div><div class="output-specification"><p>On the first line output a single integer — the answer to the given task modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span">|<i>S</i>|</span> (<span class="tex-span">1 ≤ |<i>S</i>| ≤ 1000</span>) — the number of vertices of tree <span class="tex-span"><i>S</i></span>.</p><p>Next <span class="tex-span">|<i>S</i>| - 1</span> lines contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>S</i>|</span>) and describe edges of tree <span class="tex-span"><i>S</i></span>.</p><p>The next line contains a single integer <span class="tex-span">|<i>T</i>|</span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ 12</span>) — the number of vertices of tree <span class="tex-span"><i>T</i></span>.</p><p>Next <span class="tex-span">|<i>T</i>| - 1</span> lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>T</i>|</span>) and describe edges of tree <span class="tex-span"><i>T</i></span>.</p>

## Output

<p>On the first line output a single integer — the answer to the given task modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
5
1 2
2 3
3 4
4 5
3
1 2
2 3

```




```input2
3
2 3
3 1
3
1 2
1 3

```




```input3
7
1 2
1 3
1 4
1 5
1 6
1 7
4
4 1
4 2
4 3

```




```input4
5
1 2
2 3
3 4
4 5
4
4 1
4 2
4 3

```




```output1
3

```




```output2
1

```




```output3
20

```




```output4
0

```


