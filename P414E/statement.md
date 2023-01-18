## Description

<div><p>After a lot of trying, Mashmokh designed a problem and it's your job to solve it.</p><p>You have a tree <span class="tex-span"><i>T</i></span> with <span class="tex-span"><i>n</i></span> vertices. Each vertex has a unique index from 1 to <span class="tex-span"><i>n</i></span>. The root of <span class="tex-span"><i>T</i></span> has index <span class="tex-span">1</span>. For each vertex of this tree <span class="tex-span"><i>v</i></span>, you are given a list of its children in a specific order. You must perform three types of query on this tree:</p><ol> <li> find distance (the number of edges in the shortest path) between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>; </li><li> given <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>h</i></span>, disconnect <span class="tex-span"><i>v</i></span> from its father and connect it to its <span class="tex-span"><i>h</i></span>-th ancestor; more formally, let's denote the path from <span class="tex-span"><i>v</i></span> to the root by <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>l</i></sub>&nbsp;(<i>h</i> &lt; <i>l</i>)</span>, so that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>v</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>l</i></sub></span> is root; disconnect <span class="tex-span"><i>v</i></span> from its father (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>) and connect it to <span class="tex-span"><i>x</i><sub class="lower-index"><i>h</i> + 1</sub></span>; vertex <span class="tex-span"><i>v</i></span> must be added to the end of the child-list of vertex <span class="tex-span"><i>x</i><sub class="lower-index"><i>h</i> + 1</sub></span>; </li><li> in the vertex sequence produced by calling function dfs(root) find the latest vertex that has distance <span class="tex-span"><i>k</i></span> from the root. </li></ol><p>The pseudo-code of function dfs(v): </p><pre class="verbatim"><br>// ls[v]: list of children of vertex v <br>// its i-th element is ls[v][i]<br>// its size is size(ls[v])<br>sequence result = empty sequence;<br>void dfs(vertex now)<br>{<br>    add now to end of result;<br>    for(int i = 1; i &lt;= size(ls[v]); i = i + 1) //loop from i = 1 to i = size(ls[v])<br>        dfs(ls[v][i]);<br>}<br></pre></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>&nbsp;(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of vertices of <span class="tex-span"><i>T</i></span> and number of queries to perform.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains an integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>&nbsp;(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, number of <span class="tex-span"><i>i</i></span>-th vertex's children. Then <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers follow, the <span class="tex-span"><i>j</i></span>-th of them is the index of <span class="tex-span"><i>j</i></span>-th child of <span class="tex-span"><i>i</i></span>-th vertex. Note that the order of these vertices is important.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines has one of the following format: "<span class="tex-span">1</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>u</i></span>", "<span class="tex-span">2</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>h</i></span>", or "<span class="tex-span">3</span> <span class="tex-span"><i>k</i></span>". The first number in the line is the type of query to perform according to the problem statement. The next numbers are description of the query.</p><p>It's guaranteed that all the queries are correct. For example, in the second-type query <span class="tex-span"><i>h</i></span> is at least 2 and at most distance of <span class="tex-span"><i>v</i></span> from root. Also in the third-type query there is at least one vertex with distance <span class="tex-span"><i>k</i></span> from the root at the time the query is given.</p></div><div class="output-specification"><p>For each query of the first or third type output one line containing the result of the query.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>&nbsp;(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of vertices of <span class="tex-span"><i>T</i></span> and number of queries to perform.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains an integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>&nbsp;(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, number of <span class="tex-span"><i>i</i></span>-th vertex's children. Then <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers follow, the <span class="tex-span"><i>j</i></span>-th of them is the index of <span class="tex-span"><i>j</i></span>-th child of <span class="tex-span"><i>i</i></span>-th vertex. Note that the order of these vertices is important.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines has one of the following format: "<span class="tex-span">1</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>u</i></span>", "<span class="tex-span">2</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>h</i></span>", or "<span class="tex-span">3</span> <span class="tex-span"><i>k</i></span>". The first number in the line is the type of query to perform according to the problem statement. The next numbers are description of the query.</p><p>It's guaranteed that all the queries are correct. For example, in the second-type query <span class="tex-span"><i>h</i></span> is at least 2 and at most distance of <span class="tex-span"><i>v</i></span> from root. Also in the third-type query there is at least one vertex with distance <span class="tex-span"><i>k</i></span> from the root at the time the query is given.</p>

## Output

<p>For each query of the first or third type output one line containing the result of the query.</p>





```input1
4 9
1 2
1 3
1 4
0
1 1 4
2 4 2
1 3 4
3 1
3 2
2 3 2
1 1 2
3 1
3 2

```




```input2
2 2
1 2
0
1 2 1
3 1

```




```output1
3
2
2
4
1
3
4

```




```output2
1
2

```


