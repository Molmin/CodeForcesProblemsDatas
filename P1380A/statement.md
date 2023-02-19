## Description

<div><p>You are given a permutation $p_1, p_2, \dots, p_n$. Recall that sequence of $n$ integers is called a <span class="tex-font-style-it">permutation</span> if it contains all integers from $1$ to $n$ exactly once.</p><p>Find three indices $i$, $j$ and $k$ such that: </p><ul> <li> $1 \le i &lt; j &lt; k \le n$; </li><li> $p_i &lt; p_j$ and $p_j &gt; p_k$. </li></ul> Or say that there are no such indices.</div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 200$)&nbsp;— the number of test cases.</p><p>Next $2T$ lines contain test cases&nbsp;— two lines per test case. The first line of each test case contains the single integer $n$ ($3 \le n \le 1000$)&nbsp;— the length of the permutation $p$.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$; $p_i \neq p_j$ if $i \neq j$)&nbsp;— the permutation $p$.</p></div><div class="output-specification"><p>For each test case: </p><ul> <li> if there are such indices $i$, $j$ and $k$, print <span class="tex-font-style-tt">YES</span> (case insensitive) and the indices themselves; </li><li> if there are no such indices, print <span class="tex-font-style-tt">NO</span> (case insensitive). </li></ul><p>If there are multiple valid triples of indices, print any of them.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 200$)&nbsp;— the number of test cases.</p><p>Next $2T$ lines contain test cases&nbsp;— two lines per test case. The first line of each test case contains the single integer $n$ ($3 \le n \le 1000$)&nbsp;— the length of the permutation $p$.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$; $p_i \neq p_j$ if $i \neq j$)&nbsp;— the permutation $p$.</p>

## Output

<p>For each test case: </p><ul> <li> if there are such indices $i$, $j$ and $k$, print <span class="tex-font-style-tt">YES</span> (case insensitive) and the indices themselves; </li><li> if there are no such indices, print <span class="tex-font-style-tt">NO</span> (case insensitive). </li></ul><p>If there are multiple valid triples of indices, print any of them.</p>





```input1
3
4
2 1 4 3
6
4 6 1 2 5 3
5
5 3 1 2 4
```




```output1
YES
2 3 4
YES
3 5 6
NO
```


