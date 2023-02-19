## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>Kochiya Sanae is playing with magnets. Realizing that some of those magnets are demagnetized, she is curious to find them out.</p><p>There are $n$ magnets, which can be of the following $3$ types:</p><ul><li> <span class="tex-font-style-tt">N</span> </li><li> <span class="tex-font-style-tt">S</span> </li><li> <span class="tex-font-style-tt">-</span> — these magnets are demagnetized.</li></ul> <p>Note that <span class="tex-font-style-bf">you don't know</span> the types of these magnets beforehand.</p><p>You have a machine which can measure the force between the magnets, and you can use it <span class="tex-font-style-bf">at most</span> $n+\lfloor \log_2n\rfloor$ times.</p><p>You can put some magnets to the left part of the machine and some to the right part of the machine, and launch the machine. Obviously, you can put one magnet to at most one side (you don't have to put all magnets). You can put the same magnet in different queries.</p><p>Then the machine will tell the force these magnets produce. Formally, let $n_1,s_1$ be the number of <span class="tex-font-style-tt">N</span> and <span class="tex-font-style-tt">S</span> magnets correspondently on the left and $n_2,s_2$ — on the right. Then the force between them would be $n_1n_2+s_1s_2-n_1s_2-n_2s_1$. Please note that the force is a <span class="tex-font-style-bf">signed</span> value.</p><p>However, when the <span class="tex-font-style-bf">absolute</span> value of the force is <span class="tex-font-style-bf">strictly larger than</span> $n$, the machine will crash into pieces.</p><p>You need to find <span class="tex-font-style-bf">all</span> magnets of type <span class="tex-font-style-tt">-</span> (all demagnetized ones), <span class="tex-font-style-bf">without breaking the machine</span>.</p><p><span class="tex-font-style-bf">Note that the interactor is not adaptive</span>. The types of the magnets are fixed before the start of the interaction and do not change with queries.</p><p>It is guaranteed that there are <span class="tex-font-style-bf">at least</span> $2$ magnets whose type is not <span class="tex-font-style-tt">-</span>, and <span class="tex-font-style-bf">at least</span> $1$ magnet of type <span class="tex-font-style-tt">-</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$) — the number of test cases.</p></div><div><h2>Interaction</h2><p>For each test case you should start by reading an integer $n$ ($3 \leq n \leq 2000$) — the number of the magnets. </p><p>It is guaranteed that the total sum of all $n$ over all test cases doesn't exceed $2000$.</p><p>After that you can put some magnets into the machine and make a query from the statement.</p><p>You have to print each query in three lines:</p><ul><li> In the first line print "<span class="tex-font-style-tt">? l r</span>" (without quotes) where $l$ and $r$ ($1 \leq l,r &lt; n$, $l+r \leq n$) respectively denote the number of the magnets you put to left and right.</li><li> In the second line print $l$ integers $a_1, \dots, a_l$ ($1 \leq a_i \leq n$, $a_i \neq a_j$ if $i \neq j$) — the indices of the magnets you put to left.</li><li> In the third line print $r$ integers $b_1, \dots, b_r$ ($1 \leq b_i \leq n$, $b_i \neq b_j$ if $i \neq j$) — the indices of the magnets you put to right.</li><li> The same magnet can't be put to both sides <span class="tex-font-style-bf">in the same query</span>. Formally, you should guarantee that $a_i \neq b_j$ for any $i$ and $j$. However, you may leave some magnets unused.</li></ul><p>After printing a query do not forget to <span class="tex-font-style-bf">output end of line and flush the output</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p>After this, you should read an integer $F$ — the force these magnets produce.</p><p>Note that if your query is invalid(either the query limit exceeds, the machine crashes or the arguments are invalid), <span class="tex-font-style-bf">the interactor will terminate immediately</span>. In this case terminate your program to receive verdict <span class="tex-font-style-tt">Wrong Answer</span> instead of arbitrary verdicts.</p><p>If you are confident about your answer, use the following format to report it:</p><ul><li> "<span class="tex-font-style-tt">! k A</span>", where $k$ is the number of magnets you found, and $A$ is an array consisting of $k$ different integers from $1$ to $n$ denoting the indices of the magnets of type <span class="tex-font-style-tt">-</span> that you found. You may print elements of $A$ in <span class="tex-font-style-bf">arbitrary order</span>.</li><li> After that, if this is the last test case, you have to terminate your program; otherwise you should immediately continue to deal with the next test case.</li></ul><p><span class="tex-font-style-bf">Note that the interactor is not adaptive</span>. The types of the magnets are fixed before the start of interaction and do not change with queries.</p><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack a solution, use the following format:</p><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$) — the number of test cases in your hack.</p><p>Then follow the descriptions of the $t$ test cases, each printed in two lines:</p><ul><li> The first line contains a single integer $n$ ($3 \leq n \leq 2000$) — the number of magnets.</li><li> The second line contains a string $S$ of length $n$ consisting of only <span class="tex-font-style-tt">N</span>, <span class="tex-font-style-tt">S</span> and <span class="tex-font-style-tt">-</span>, denoting the magnets' types.</li><li> Each of your test case should guarantee that there are <span class="tex-font-style-bf">at least</span> $2$ magnets whose type is not <span class="tex-font-style-tt">-</span>, and <span class="tex-font-style-bf">at least</span> $1$ magnet of type <span class="tex-font-style-tt">-</span>. Meanwhile, the total sum of $n$ in all test cases should not exceed $2000$.</li></ul></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$) — the number of test cases.</p>





```input1
1
4



0



1



0



0
```




```output1
? 1 1
3
4

? 1 2
1
2 3

? 1 1
1
4

? 1 1
1
3

! 2 3 4
```



## Note

<p>The empty lines in the sample are just for you to better understand the interaction process. <span class="tex-font-style-bf">You're not required to print them</span>.</p><p>In the sample, the types of the magnets are <span class="tex-font-style-tt">NN</span><span class="tex-font-style-tt">-</span><span class="tex-font-style-tt">-</span>.</p><p>At first, you put the third magnet on the left and the fourth one on the right. Both of them have type <span class="tex-font-style-tt">-</span>, thus no force is produced.</p><p>Then you put the first magnet on the left and the second and third one on the right. The third magnet has type <span class="tex-font-style-tt">-</span>, while the other two magnets are of type <span class="tex-font-style-tt">N</span>, so the force produced is $1$.</p><p>In the following two queries, the force is $0$ since there is only a magnet with property <span class="tex-font-style-tt">-</span> on the right.</p><p>Then we can determine that the magnets of type <span class="tex-font-style-tt">-</span> are the third and the fourth one, so we should print <span class="tex-font-style-tt">! 2 3 4</span> and exit.</p>
