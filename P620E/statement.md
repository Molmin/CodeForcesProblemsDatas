## Description

<div><p>The New Year holidays are over, but Resha doesn't want to throw away the New Year tree. He invited his best friends Kerim and Gural to help him to redecorate the New Year tree.</p><p>The New Year tree is an undirected tree with <span class="tex-span"><i>n</i></span> vertices and root in the vertex <span class="tex-span">1</span>.</p><p>You should process the queries of the two types:</p><ol> <li> Change the colours of all vertices in the subtree of the vertex <span class="tex-span"><i>v</i></span> to the colour <span class="tex-span"><i>c</i></span>. </li><li> Find the number of different colours in the subtree of the vertex <span class="tex-span"><i>v</i></span>. </li></ol></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 4·10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree and the number of the queries.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 60</span>) — the colour of the <span class="tex-span"><i>i</i></span>-th vertex.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the vertices of the <span class="tex-span"><i>j</i></span>-th edge. It is guaranteed that you are given correct undirected tree.</p><p>The last <span class="tex-span"><i>m</i></span> lines contains the description of the queries. Each description starts with the integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>k</i></sub> ≤ 2</span>) — the type of the <span class="tex-span"><i>k</i></span>-th query. For the queries of the first type then follows two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub>, <i>c</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>k</i></sub> ≤ 60</span>) — the number of the vertex whose subtree will be recoloured with the colour <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span>. For the queries of the second type then follows integer <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>) — the number of the vertex for which subtree you should find the number of different colours.</p></div><div class="output-specification"><p>For each query of the second type print the integer <span class="tex-span"><i>a</i></span> — the number of different colours in the subtree of the vertex given in the query.</p><p>Each of the numbers should be printed on a separate line in order of query appearing in the input.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 4·10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree and the number of the queries.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 60</span>) — the colour of the <span class="tex-span"><i>i</i></span>-th vertex.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the vertices of the <span class="tex-span"><i>j</i></span>-th edge. It is guaranteed that you are given correct undirected tree.</p><p>The last <span class="tex-span"><i>m</i></span> lines contains the description of the queries. Each description starts with the integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>k</i></sub> ≤ 2</span>) — the type of the <span class="tex-span"><i>k</i></span>-th query. For the queries of the first type then follows two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub>, <i>c</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>k</i></sub> ≤ 60</span>) — the number of the vertex whose subtree will be recoloured with the colour <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span>. For the queries of the second type then follows integer <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>) — the number of the vertex for which subtree you should find the number of different colours.</p>

## Output

<p>For each query of the second type print the integer <span class="tex-span"><i>a</i></span> — the number of different colours in the subtree of the vertex given in the query.</p><p>Each of the numbers should be printed on a separate line in order of query appearing in the input.</p>





```input1
7 10
1 1 1 1 1 1 1
1 2
1 3
1 4
3 5
3 6
3 7
1 3 2
2 1
1 4 3
2 1
1 2 5
2 1
1 6 4
2 1
2 2
2 3

```




```input2
23 30
1 2 2 6 5 3 2 1 1 1 2 4 5 3 4 4 3 3 3 3 3 4 6
1 2
1 3
1 4
2 5
2 6
3 7
3 8
4 9
4 10
4 11
6 12
6 13
7 14
7 15
7 16
8 17
8 18
10 19
10 20
10 21
11 22
11 23
2 1
2 5
2 6
2 7
2 8
2 9
2 10
2 11
2 4
1 12 1
1 13 1
1 14 1
1 15 1
1 16 1
1 17 1
1 18 1
1 19 1
1 20 1
1 21 1
1 22 1
1 23 1
2 1
2 5
2 6
2 7
2 8
2 9
2 10
2 11
2 4

```




```output1
2
3
4
5
1
2

```




```output2
6
1
3
3
2
1
2
3
5
5
1
2
2
1
1
1
2
3

```


