## Description

<div><p>You have a root tree containing <span class="tex-span"><i>n</i></span> vertexes. Let's number the tree vertexes with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The tree root is in the vertex <span class="tex-span">1</span>.</p><p>Each vertex (except fot the tree root) <span class="tex-span"><i>v</i></span> has a direct ancestor <span class="tex-span"><i>p</i><sub class="lower-index"><i>v</i></sub></span>. Also each vertex <span class="tex-span"><i>v</i></span> has its integer value <span class="tex-span"><i>s</i><sub class="lower-index"><i>v</i></sub></span>. </p><p>Your task is to perform following queries:</p><ul> <li> <span class="tex-font-style-bf">P</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>u</i></span> (<span class="tex-span"><i>u</i> ≠ <i>v</i></span>). If <span class="tex-span"><i>u</i></span> isn't in subtree of <span class="tex-span"><i>v</i></span>, you must perform the assignment <span class="tex-span"><i>p</i><sub class="lower-index"><i>v</i></sub> = <i>u</i></span>. Otherwise you must perform assignment <span class="tex-span"><i>p</i><sub class="lower-index"><i>u</i></sub> = <i>v</i></span>. Note that after this query the graph continues to be a tree consisting of <span class="tex-span"><i>n</i></span> vertexes.</li><li> <span class="tex-font-style-bf">V</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>t</i></span>. Perform assignment <span class="tex-span"><i>s</i><sub class="lower-index"><i>v</i></sub> = <i>t</i></span>. </li></ul><p>Your task is following. Before starting performing queries and after each query you have to calculate expected value written on the lowest common ancestor of two equiprobably selected vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. Here lowest common ancestor of <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> is the deepest vertex that lies on the both of the path from the root to vertex <span class="tex-span"><i>i</i></span> and the path from the root to vertex <span class="tex-span"><i>j</i></span>. Please note that the vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> can be the same (in this case their lowest common ancestor coincides with them).</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>) — the number of the tree vertexes. </p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integer <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the description of the tree edges. It is guaranteed that those numbers form a tree.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers — <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ... <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the values written on each vertex of the tree.</p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">4</sup></span>) — the number of queries. Each of the following <span class="tex-span"><i>q</i></span> lines contains the description of the query in the format described in the statement. It is guaranteed that query arguments <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> lie between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>. It is guaranteed that argument <span class="tex-span"><i>t</i></span> in the queries of type <span class="tex-font-style-bf">V</span> meets limits <span class="tex-span">0 ≤ <i>t</i> ≤ 10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i> + 1</span> number — the corresponding expected values. Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>) — the number of the tree vertexes. </p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integer <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the description of the tree edges. It is guaranteed that those numbers form a tree.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers — <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ... <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the values written on each vertex of the tree.</p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">4</sup></span>) — the number of queries. Each of the following <span class="tex-span"><i>q</i></span> lines contains the description of the query in the format described in the statement. It is guaranteed that query arguments <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> lie between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>. It is guaranteed that argument <span class="tex-span"><i>t</i></span> in the queries of type <span class="tex-font-style-bf">V</span> meets limits <span class="tex-span">0 ≤ <i>t</i> ≤ 10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Print <span class="tex-span"><i>q</i> + 1</span> number — the corresponding expected values. Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
5
1 2 2 1
1 2 3 4 5
5
P 3 4
P 4 5
V 2 3
P 5 2
P 1 4

```




```output1
1.640000000
1.800000000
2.280000000
2.320000000
2.800000000
1.840000000

```



## Note

<p>Note that in the query <span class="tex-font-style-bf">P</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>u</i></span> if <span class="tex-span"><i>u</i></span> lies in subtree of <span class="tex-span"><i>v</i></span> you must perform assignment <span class="tex-span"><i>p</i><sub class="lower-index"><i>u</i></sub> = <i>v</i></span>. An example of such case is the last query in the sample.</p>
