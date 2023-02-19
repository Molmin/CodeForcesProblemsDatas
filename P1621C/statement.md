## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>The jury has a permutation $p$ of length $n$ and wants you to guess it. For this, the jury created another permutation $q$ of length $n$. Initially, $q$ is an identity permutation ($q_i = i$ for all $i$).</p><p>You can ask queries to get $q_i$ for any $i$ you want. After each query, the jury will change $q$ in the following way: </p><ul> <li> At first, the jury will create a new permutation $q'$ of length $n$ such that $q'_i = q_{p_i}$ for all $i$. </li><li> Then the jury will replace permutation $q$ with pemutation $q'$. </li></ul><p>You can make no more than $2n$ queries in order to quess $p$.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p></div><div><h2>Interaction</h2><p>Interaction in each test case starts after reading the single integer $n$ ($1 \leq n \leq 10^4$)&nbsp;— the length of permutations $p$ and $q$.</p><p>To get the value of $q_i$, output the query in the format $?$ $i$ ($1 \leq i \leq n$). After that you will receive the value of $q_i$.</p><p>You can make at most $2n$ queries. After the incorrect query you will receive $0$ and you should exit immediately to get <span class="tex-font-style-tt">Wrong answer</span> verdict.</p><p>When you will be ready to determine $p$, output $p$ in format $!$ $p_1$ $p_2$ $\ldots$ $p_n$. After this you should go to the next test case or exit if it was the last test case. Printing the permutation is not counted as one of $2n$ queries.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^4$. The interactor is not adaptive in this problem.</p><p><span class="tex-font-style-bf">Hacks:</span></p><p>To hack, use the following format:</p><p>The first line contains the single integer $t$&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$&nbsp;— the length of the permutations $p$ and $q$. The second line of each test case contains $n$ integers $p_1, p_2, \ldots, p_n$&nbsp;— the hidden permutation for this test case.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p>





```input1
2
4

3

2

1

4

2

4

4
```




```output1
? 3

? 2

? 4

! 4 2 1 3

? 2

? 3

? 2

! 1 3 4 2
```



## Note

<p>In the first test case the hidden permutation $p = [4, 2, 1, 3]$.</p><p>Before the first query $q = [1, 2, 3, 4]$ so answer for the query will be $q_3 = 3$.</p><p>Before the second query $q = [4, 2, 1, 3]$ so answer for the query will be $q_2 = 2$.</p><p>Before the third query $q = [3, 2, 4, 1]$ so answer for the query will be $q_4 = 1$.</p><p>In the second test case the hidden permutation $p = [1, 3, 4, 2]$.</p><p>Empty strings are given only for better readability. There will be no empty lines in the testing system.</p>
