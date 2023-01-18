## Description

<div><p><span class="tex-font-style-it">This is an interactive problem!</span></p><p>An arithmetic progression or arithmetic sequence is a sequence of integers such that the subtraction of element with its previous element ($x_i - x_{i - 1}$, where $i \ge 2$) is constant&nbsp;— such difference is called a <span class="tex-font-style-it">common difference</span> of the sequence.</p><p>That is, an arithmetic progression is a sequence of form $x_i = x_1 + (i - 1) d$, where $d$ is a common difference of the sequence.</p><p>There is a secret list of $n$ integers $a_1, a_2, \ldots, a_n$.</p><p>It is guaranteed that all elements $a_1, a_2, \ldots, a_n$ are between $0$ and $10^9$, inclusive.</p><p>This list is special: if sorted in increasing order, it will form an arithmetic progression with positive common difference ($d &gt; 0$). For example, the list $[14, 24, 9, 19]$ satisfies this requirement, after sorting it makes a list $[9, 14, 19, 24]$, which can be produced as $x_n = 9 + 5 \cdot (n - 1)$.</p><p>Also you are also given a device, which has a quite discharged battery, thus you can only use it to perform at most $60$ queries of following two types:</p><ul><li> Given a value $i$ ($1 \le i \le n$), the device will show the value of the $a_i$.</li><li> Given a value $x$ ($0 \le x \le 10^9$), the device will return $1$ if an element with a value strictly greater than $x$ exists, and it will return $0$ otherwise.</li></ul><p>Your can use this special device for at most $60$ queries. Could you please find out the smallest element and the common difference of the sequence? That is, values $x_1$ and $d$ in the definition of the arithmetic progression. Note that the array $a$ is not sorted.</p></div><div><h2>Interaction</h2><p>The interaction starts with a single integer $n$ ($2 \le n \le 10^6$), the size of the list of integers.</p><p>Then you can make queries of two types:</p><ul><li> "<span class="tex-font-style-tt">? i</span>" ($1 \le i \le n$)&nbsp;— to get the value of $a_i$.</li><li> "<span class="tex-font-style-tt">&gt; x</span>" ($0 \le x \le 10^9$)&nbsp;— to check whether there exists an element greater than $x$</li></ul><p>After the query read its result $r$ as an integer.</p><ul> <li> For the first query type, the $r$ satisfies $0 \le r \le 10^9$. </li><li> For the second query type, the $r$ is either $0$ or $1$.</li><li> In case you make more than $60$ queries or violated the number range in the queries, you will get a $r = -1$.</li><li> If you terminate after receiving the <span class="tex-font-style-tt">-1</span>, you will get the "<span class="tex-font-style-tt">Wrong answer</span>" verdict. Otherwise you can get an arbitrary verdict because your solution will continue to read from a closed stream. </li></ul><p>When you find out what the smallest element $x_1$ and common difference $d$, print</p><ul> <li> "<span class="tex-font-style-tt">! $x_1$ $d$</span>" </li></ul><p>And quit after that. This query is not counted towards the $60$ queries limit.</p><p>After printing any query do not forget to output end of line and flush the output. Otherwise you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>For hack, use the following format:</p><p>The first line should contain an integer $n$ ($2 \le n \le 10^6$)&nbsp;— the list's size.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the elements of the list.</p><p>Also, after the sorting the list must form an arithmetic progression with positive common difference.</p></div>





```input1
4

0

1

14

24

9

19
```




```output1
&gt; 25

&gt; 15

? 1

? 2

? 3

? 4

! 9 5
```



## Note

<p>Note that the example interaction contains extra empty lines so that it's easier to read. The real interaction doesn't contain any empty lines and you shouldn't print any extra empty lines as well.</p><p>The list in the example test is $[14, 24, 9, 19]$.</p>
