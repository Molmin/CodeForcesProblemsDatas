## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>After getting AC after 13 Time Limit Exceeded verdicts on a geometry problem, Kuroni went to an Italian restaurant to celebrate this holy achievement. Unfortunately, the excess sauce disoriented him, and he's now lost!</p><p>The United States of America can be modeled as a tree (why though) with $n$ vertices. The tree is rooted at vertex $r$, wherein lies Kuroni's hotel.</p><p>Kuroni has a phone app designed to help him in such emergency cases. To use the app, he has to input two vertices $u$ and $v$, and it'll return a vertex $w$, which is the lowest common ancestor of those two vertices.</p><p>However, since the phone's battery has been almost drained out from live-streaming Kuroni's celebration party, he could only use the app at most $\lfloor \frac{n}{2} \rfloor$ times. After that, the phone would die and there will be nothing left to help our dear friend! :(</p><p>As the night is cold and dark, Kuroni needs to get back, so that he can reunite with his comfy bed and pillow(s). Can you help him figure out his hotel's location?</p></div><div><h2>Interaction</h2><p>The interaction starts with reading a single integer $n$ ($2 \le n \le 1000$), the number of vertices of the tree.</p><p>Then you will read $n-1$ lines, the $i$-th of them has two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$, $x_i \ne y_i$), denoting there is an edge connecting vertices $x_i$ and $y_i$. It is guaranteed that the edges will form a tree.</p><p>Then you can make queries of type "<span class="tex-font-style-tt">? u v</span>" ($1 \le u, v \le n$) to find the lowest common ancestor of vertex $u$ and $v$.</p><p>After the query, read the result $w$ as an integer.</p><p>In case your query is invalid or you asked more than $\lfloor \frac{n}{2} \rfloor$ queries, the program will print $-1$ and will finish interaction. You will receive a <span class="tex-font-style-bf">Wrong answer</span> verdict. Make sure to exit immediately to avoid getting other verdicts.</p><p>When you find out the vertex $r$, print "<span class="tex-font-style-tt">! $r$</span>" and quit after that. This query does not count towards the $\lfloor \frac{n}{2} \rfloor$ limit.</p><p>Note that the tree is fixed beforehand and will not change during the queries, i.e. the interactor is not adaptive.</p><p>After printing any query do not forget to print end of line and flush the output. Otherwise, you might get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack, use the following format:</p><p>The first line should contain two integers $n$ and $r$ ($2 \le n \le 1000$, $1 \le r \le n$), denoting the number of vertices and the vertex with Kuroni's hotel.</p><p>The $i$-th of the next $n-1$ lines should contain two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$)&nbsp;— denoting there is an edge connecting vertex $x_i$ and $y_i$.</p><p>The edges presented should form a tree.</p></div>





```input1
6
1 4
4 2
5 3
6 3
2 3

3

4

4
```




```output1
? 5 6

? 3 1

? 1 2

! 4
```



## Note

<p>Note that the example interaction contains extra empty lines so that it's easier to read. The real interaction doesn't contain any empty lines and you shouldn't print any extra empty lines as well.</p><p>The image below demonstrates the tree in the sample test:</p><p><img class="tex-graphics" src="file://6sbVNF19.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
