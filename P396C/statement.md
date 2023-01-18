## Description

<div><p>You are given a rooted tree consisting of <span class="tex-span"><i>n</i></span> vertices numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The root of the tree is a vertex number <span class="tex-span">1</span>.</p><p>Initially all vertices contain number <span class="tex-span">0</span>. Then come <span class="tex-span"><i>q</i></span> queries, each query has one of the two types:</p><ul> <li> The format of the query: <span class="tex-span">1</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>k</i></span>. In response to the query, you need to add to the number at vertex <span class="tex-span"><i>v</i></span> number <span class="tex-span"><i>x</i></span>; to the numbers at the <span class="tex-font-style-bf">descendants</span> of vertex <span class="tex-span"><i>v</i></span> at distance <span class="tex-span">1</span>, add <span class="tex-span"><i>x</i> - <i>k</i></span>; and so on, to the numbers written in the descendants of vertex <span class="tex-span"><i>v</i></span> at distance <span class="tex-span"><i>i</i></span>, you need to add <span class="tex-span"><i>x</i> - (<i>i</i>·<i>k</i>)</span>. The distance between two vertices is the number of edges in the shortest path between these vertices. </li><li> The format of the query: <span class="tex-span">2</span> <span class="tex-span"><i>v</i></span>. In reply to the query you should print the number written in vertex <span class="tex-span"><i>v</i></span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. </li></ul><p>Process the queries given in the input.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) —&nbsp;the number of vertices in the tree. The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ... <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the number of the vertex that is the parent of vertex <span class="tex-span"><i>i</i></span> in the tree.</p><p>The third line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain the queries, one per line. The first number in the line is <span class="tex-span"><i>type</i></span>. It represents the type of the query. If <span class="tex-span"><i>type</i> = 1</span>, then next follow space-separated integers <span class="tex-span"><i>v</i>, <i>x</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>; <span class="tex-span">0 ≤ <i>x</i> &lt; 10<sup class="upper-index">9</sup> + 7</span>; <span class="tex-span">0 ≤ <i>k</i> &lt; 10<sup class="upper-index">9</sup> + 7</span>). If <span class="tex-span"><i>type</i> = 2</span>, then next follows integer <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>) —&nbsp;the vertex where you need to find the value of the number.</p></div><div class="output-specification"><p>For each query of the second type print on a single line the number written in the vertex from the query. Print the number modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) —&nbsp;the number of vertices in the tree. The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ... <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the number of the vertex that is the parent of vertex <span class="tex-span"><i>i</i></span> in the tree.</p><p>The third line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain the queries, one per line. The first number in the line is <span class="tex-span"><i>type</i></span>. It represents the type of the query. If <span class="tex-span"><i>type</i> = 1</span>, then next follow space-separated integers <span class="tex-span"><i>v</i>, <i>x</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>; <span class="tex-span">0 ≤ <i>x</i> &lt; 10<sup class="upper-index">9</sup> + 7</span>; <span class="tex-span">0 ≤ <i>k</i> &lt; 10<sup class="upper-index">9</sup> + 7</span>). If <span class="tex-span"><i>type</i> = 2</span>, then next follows integer <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>) —&nbsp;the vertex where you need to find the value of the number.</p>

## Output

<p>For each query of the second type print on a single line the number written in the vertex from the query. Print the number modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
3
1 1
3
1 1 2 1
2 1
2 2

```




```output1
2
1

```



## Note

<p>You can read about a rooted tree here: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Tree_(graph_theory)</span>.</p>
