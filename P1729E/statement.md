## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem</span>.</p><p><span class="tex-font-style-it">I want to play a game with you...</span></p><p>We hid from you a cyclic graph of $n$ vertices ($3 \le n \le 10^{18}$). A cyclic graph is an undirected graph of $n$ vertices that form one cycle. Each vertex belongs to the cycle, i.e. the length of the cycle (the number of edges in it) is exactly $n$. The order of the vertices in the cycle is arbitrary.</p><p>You can make queries in the following way:</p><ul><li> "<span class="tex-font-style-tt">? a b</span>" where $1 \le a, b \le 10^{18}$ and $a \neq b$. In response to the query, the interactor outputs on a separate line the length of random of two paths from vertex $a$ to vertex $b$, or <span class="tex-font-style-tt">-1</span> if $\max(a, b) &gt; n$. The interactor chooses one of the two paths with <span class="tex-font-style-bf">equal probability</span>. The length of the path&nbsp;—is the number of edges in it.</li></ul><p>You win if you guess the number of vertices in the hidden graph (number $n$) by making no more than $50$ queries.</p><p>Note that the interactor is implemented in such a way that for any ordered pair $(a, b)$, it always returns the same value for query "<span class="tex-font-style-tt">? a b</span>", no matter how many such queries. Note that the "<span class="tex-font-style-tt">? b a</span>" query may be answered differently by the interactor.</p><p>The vertices in the graph are randomly placed, and their positions are fixed in advance.</p><p>Hacks are forbidden in this problem. The number of tests the jury has is $50$.</p></div><div><h2>Interaction</h2><p>You can make no more than $50$ of queries. To make a query, output on a separate line:</p><ul> <li> "<span class="tex-font-style-tt">? a b</span>", where $1 \le a, b \le 10^{18}$ and $a \neq b$. In response to the query, the interactor will output on a separate line the length of a random simple path from vertex $a$ to vertex $b$ (not to be confused with the path from $b$ to $a$), or $-1$ if $\max(a, b) &gt; n$. The interactor chooses one of the two paths with <span class="tex-font-style-bf">equal probability</span>. </li></ul><p>If your program gets a number <span class="tex-font-style-tt">0</span> as a result of a query, it means that the verdict for your solution is already defined as "<span class="tex-font-style-it">wrong answer</span>" (for example, you made more than $50$ queries or made an invalid query). In this case, your program should terminate immediately. Otherwise, in this scenario you may get a random verdict "<span class="tex-font-style-it">Execution error</span>", "<span class="tex-font-style-it">Exceeded time limit</span>" or some other verdict instead of "<span class="tex-font-style-it">Wrong answer</span>".</p><p>The answer, like queries, print on a separate line. The output of the answer is not counted as a query when counting them. To print it, use the following format:</p><ul> <li> "<span class="tex-font-style-tt">! n</span>": the expected size of the hidden graph ($3 \le n \le 10^{18}$). </li></ul><p>After that, your program should terminate.</p><p>After the output of the next query, be sure to use stream cleaning functions so that some of your output is not left in some buffer. For example, in C++ you should use function <span class="tex-font-style-tt">flush(stdout)</span>, in Java call <span class="tex-font-style-tt">System.out.flush()</span>, in Pascal <span class="tex-font-style-tt">flush(output)</span> and <span class="tex-font-style-tt">stdout.flush()</span> for Python.</p><p>Note that the interactor is implemented in such a way that for any ordered pair $(a, b)$, it always returns the same value for query "<span class="tex-font-style-tt">? a b</span>", no matter how many such queries. Note that the "<span class="tex-font-style-tt">? b a</span>" query may be answered differently by the interactor.</p><p>The vertices in the graph are randomly placed, and their positions are fixed in advance.</p><p>Hacks are forbidden in this problem. The number of tests the jury has is $50$.</p></div>





```input1
1

2

-1
```




```output1
? 1 2

? 1 3

? 1 4

! 3
```



## Note

<p>In the first example, the graph could look like this</p><center> <img class="tex-graphics" src="file://GmiZM58D.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The lengths of the simple paths between all pairs of vertices in this case are $1$ or $2$. </p><ul> <li> The first query finds out that one of the simple paths from vertex $1$ to vertex $2$ has a length of $1$. </li><li> With the second query, we find out that one of the simple paths from vertex $1$ to vertex $3$ has length $2$. </li><li> In the third query, we find out that vertex $4$ is not in the graph. Consequently, the size of the graph is $3$. </li></ul>
