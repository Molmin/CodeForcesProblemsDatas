## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://www.youtube.com/watch?v=5VleIdkEeak"><span class="tex-font-style-it">MisoilePunch♪ - 彩</span></a></div></div><p><span class="tex-font-style-it">This is an interactive problem!</span></p><p>On a normal day at the hidden office in A.R.C. Markland-N, Rin received an artifact, given to her by the exploration captain Sagar.</p><p>After much analysis, she now realizes that this artifact contains data about a strange flower, which has existed way before the New Age. However, the information about its chemical structure has been encrypted heavily.</p><p>The chemical structure of this flower can be represented as a string $p$. From the unencrypted papers included, Rin already knows the length $n$ of that string, and she can also conclude that the string contains at most three distinct letters: "<span class="tex-font-style-tt">C</span>" (as in Carbon), "<span class="tex-font-style-tt">H</span>" (as in Hydrogen), and "<span class="tex-font-style-tt">O</span>" (as in Oxygen).</p><p>At each moment, Rin can input a string $s$ of an arbitrary length into the artifact's terminal, and it will return every starting position of $s$ as a <span class="tex-font-style-it">substring</span> of $p$.</p><p>However, the artifact has limited energy and cannot be recharged in any way, since the technology is way too ancient and is incompatible with any current A.R.C.'s devices. To be specific:</p><ul> <li> The artifact only contains $\frac{7}{5}$ units of energy. </li><li> For each time Rin inputs a string $s$ of length $t$, the artifact consumes $\frac{1}{t^2}$ units of energy. </li><li> If the amount of energy reaches below zero, the task will be considered failed immediately, as the artifact will go black forever. </li></ul><p>Since the artifact is so precious yet fragile, Rin is very nervous to attempt to crack the final data. Can you give her a helping hand?</p></div><div><h2>Interaction</h2><p>The interaction starts with a single integer $t$ ($1 \le t \le 500$), the number of test cases. The interaction for each testcase is described below:</p><p>First, read an integer $n$ ($4 \le n \le 50$), the length of the string $p$.</p><p>Then you can make queries of type "<span class="tex-font-style-tt">? s</span>" ($1 \le |s| \le n$) to find the occurrences of $s$ as a substring of $p$.</p><p>After the query, you need to read its result as a series of integers in a line:</p><ul><li> The first integer $k$ denotes the number of occurrences of $s$ as a substring of $p$ ($-1 \le k \le n$). If $k = -1$, it means you have exceeded the energy limit or printed an invalid query, and you need to terminate immediately, to guarantee a "<span class="tex-font-style-tt">Wrong answer</span>" verdict, otherwise you might get an arbitrary verdict because your solution will continue to read from a closed stream.</li><li> The following $k$ integers $a_1, a_2, \ldots, a_k$ ($1 \le a_1 &lt; a_2 &lt; \ldots &lt; a_k \le n$) denote the starting positions of the substrings that match the string $s$.</li></ul><p>When you find out the string $p$, print "<span class="tex-font-style-tt">! $p$</span>" to finish a test case. This query doesn't consume any energy. The interactor will return an integer $1$ or $0$. If the interactor returns $1$, you can proceed to the next test case, or terminate the program if it was the last testcase.</p><p>If the interactor returns $0$, it means that your guess is incorrect, and you should to terminate to guarantee a "<span class="tex-font-style-tt">Wrong answer</span>" verdict.</p><p>Note that in every test case the string $p$ is fixed beforehand and will not change during the queries, i.e. the interactor is not adaptive.</p><p>After printing any query do not forget to print end of line and flush the output. Otherwise, you might get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>For hack, use the following format. Note that you can only hack with one test case:</p><p>The first line should contain a single integer $t$ ($t = 1$).</p><p>The second line should contain an integer $n$ ($4 \le n \le 50$)&nbsp;— the string's size.</p><p>The third line should contain a string of size $n$, consisting of characters "<span class="tex-font-style-tt">C</span>", "<span class="tex-font-style-tt">H</span>" and "<span class="tex-font-style-tt">O</span>" only. This is the string contestants will have to find out.</p></div>





```input1
1
4

2 1 2

1 2

0

1
```




```input2
2
5

0

2 2 3

1
8

1 5

1 5

1 3

2 1 2

1
```




```output1
? C

? CH

? CCHO

! CCHH
```




```output2
? O

? HHH

! CHHHH


? COO

? COOH

? HCCOO

? HH

! HHHCCOOH
```



## Note

<p>Note that the example interaction contains extra empty lines so that it's easier to read. The real interaction doesn't contain any empty lines and you shouldn't print any extra empty lines as well.</p>
