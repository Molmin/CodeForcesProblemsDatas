## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>There is a secret permutation $p$ ($1$-indexed) of numbers from $1$ to $n$. More formally, for $1 \leq i \leq n$, $1 \leq p[i] \leq n$ and for $1 \leq i &lt; j \leq n$, $p[i] \neq p[j]$. <span class="tex-font-style-bf">It is known that $p[1]&lt;p[2]$</span>.</p><p>In $1$ query, you give $3$ <span class="tex-font-style-bf">distinct</span> integers $a,b,c$ ($1 \leq a,b,c \leq n$), and receive the <span class="tex-font-style-bf">median</span> of $\{|p[a]-p[b]|,|p[b]-p[c]|,|p[a]-p[c]|\}$.</p><p>In this case, the median is the $2$-nd element ($1$-indexed) of the sequence when sorted in non-decreasing order. The median of $\{4,6,2\}$ is $4$ and the median of $\{0,123,33\}$ is $33$.</p><p>Can you find the secret permutation in not more than $2n+420$ queries?</p><p><span class="tex-font-style-bf">Note: the grader is not adaptive:</span> the permutation is fixed before any queries are made.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ $(1 \leq t \leq 1000)$ — the number of testcases.</p><p>The first line of each testcase consists of a single integer $n$ $(20 \leq n \leq 100000)$ — the length of the secret permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100000$.</p></div><div><h2>Interaction</h2><p>For each testcase, you begin the interaction by reading $n$.</p><p>To perform a query, output "<span class="tex-font-style-tt">? a b c</span>" where $a,b,c$ is the $3$ indices you want to use for the query.</p><p>Numbers have to satisfy $1 \leq a,b,c \leq n$ and $a \neq b$,$b \neq c$,$a \neq c$.</p><p>For each query, you will receive a single integer $x$: the <span class="tex-font-style-bf">median</span> of $\{|p[a]-p[b]|,|p[b]-p[c]|,|p[a]-p[c]|\}$.</p><p>In case your query is invalid or you asked more than $2n+420$ queries, the interactor will print "<span class="tex-font-style-tt">−1</span>" and will finish interaction. You will receive <span class="tex-font-style-bf">Wrong answer</span> verdict. Make sure to exit immediately to avoid getting other verdicts.</p><p>When you have determined the secret permutation, output "<span class="tex-font-style-tt">! p[1] p[2] ... p[n]</span>". If the secret permutation is correct, the interactor will print "<span class="tex-font-style-tt">1</span>". Otherwise, the interactor will print "<span class="tex-font-style-tt">-1</span>" and will finish interaction. You will receive <span class="tex-font-style-bf">Wrong answer</span> verdict. Make sure to exit immediately to avoid getting other verdicts.</p><p>After printing a query do not forget to output the end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span> verdict.</p><p>To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks:</span></p><p>To hack, use the following format of test:</p><p> The first line should contain a single integer $t$ ($1 \leq t \leq 1000$) — the number of testcases.</p><p>The first line of each testcase should contain a single integer $n$ ($20 \leq n \leq 100000$) — the length of the secret permutation.</p><p>The following line of should contain $n$ integers $p[1],p[2],p[3],\ldots,p[n]$. $p[1]&lt;p[2]$ and $p$ must be a permutation of integers from $1$ to $n$.</p><p>You must ensure that the sum of $n$ over all testcases does not exceed $100000$.</p></div>

## Input

<p>The first line of input contains a single integer $t$ $(1 \leq t \leq 1000)$ — the number of testcases.</p><p>The first line of each testcase consists of a single integer $n$ $(20 \leq n \leq 100000)$ — the length of the secret permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100000$.</p>





```input1
1
20

6

9

1
```




```output1
? 1 5 2

? 20 19 2

! 9 10 19 7 16 18 11 14 15 6 20 8 17 4 5 3 12 2 13 1
```



## Note

<p>The secret permutation is $\{9,10,19,7,16,18,11,14,15,6,20,8,17,4,5,3,12,2,13,1\}$.</p><p>For the first query, the values of $(a,b,c)$ is $(1,5,2)$. Since $p[1]=9$, $p[5]=16$ and $p[2]=10$. The return value is the median of $\{|9-16|,|16-10|,|9-10|\}$ which is $6$.</p><p>For the second query, the values of $(a,b,c)$ is $(20,19,2)$. Since $p[20]=1$, $p[19]=13$ and $p[2]=10$. The return value is the median of $\{|1-13|,|13-10|,|1-10|\}$ which is $9$.</p><p>By some miracle, we have figured out that the secret permutation is $\{9,10,19,7,16,18,11,14,15,6,20,8,17,4,5,3,12,2,13,1\}$. We output it and receive $1$ from the interactor, meaning that we have guessed the secret permutation correctly.</p>
