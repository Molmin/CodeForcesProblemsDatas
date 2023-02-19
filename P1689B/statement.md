## Description

<div><p><span class="tex-font-style-it">Monocarp is a little boy who lives in Byteland and he loves programming.</span></p><p>Recently, he found a permutation of length $n$. He has to come up with a <span class="tex-font-style-it">mystic</span> permutation. It has to be a new permutation such that it differs from the old one in each position.</p><p>More formally, if the old permutation is $p_1,p_2,\ldots,p_n$ and the new one is $q_1,q_2,\ldots,q_n$ it must hold that $$p_1\neq q_1, p_2\neq q_2, \ldots ,p_n\neq q_n.$$</p><p>Monocarp is afraid of lexicographically large permutations. Can you please help him to find the lexicographically minimal <span class="tex-font-style-it">mystic</span> permutation?</p></div><div class="input-specification"><p>There are several test cases in the input data. The first line contains a single integer $t$ ($1\leq t\leq 200$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains a positive integer $n$ ($1\leq n\leq 1000$)&nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ distinct positive integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$). It's guaranteed that $p$ is a permutation, i.&nbsp;e. $p_i \neq p_j$ for all $i \neq j$. </p><p>It is guaranteed that the sum of $n$ does not exceed $1000$ over all test cases.</p></div><div class="output-specification"><p>For each test case, output $n$ positive integers&nbsp;— the lexicographically minimal mystic permutations. If such a permutation does not exist, output $-1$ instead.</p></div>

## Input

<p>There are several test cases in the input data. The first line contains a single integer $t$ ($1\leq t\leq 200$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains a positive integer $n$ ($1\leq n\leq 1000$)&nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ distinct positive integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$). It's guaranteed that $p$ is a permutation, i.&nbsp;e. $p_i \neq p_j$ for all $i \neq j$. </p><p>It is guaranteed that the sum of $n$ does not exceed $1000$ over all test cases.</p>

## Output

<p>For each test case, output $n$ positive integers&nbsp;— the lexicographically minimal mystic permutations. If such a permutation does not exist, output $-1$ instead.</p>





```input1|2,3,6,7
4
3
1 2 3
5
2 3 4 5 1
4
2 3 1 4
1
1
```




```output1
2 3 1
1 2 3 4 5
1 2 4 3
-1
```



## Note

<p>In the first test case possible permutations that are mystic are $[2,3,1]$ and $[3,1,2]$. Lexicographically smaller of the two is $[2,3,1]$.</p><p>In the second test case, $[1,2,3,4,5]$ is the lexicographically minimal permutation and it is also mystic.</p><p>In third test case possible mystic permutations are $[1,2,4,3]$, $[1,4,2,3]$, $[1,4,3,2]$, $[3,1,4,2]$, $[3,2,4,1]$, $[3,4,2,1]$, $[4,1,2,3]$, $[4,1,3,2]$ and $[4,3,2,1]$. The smallest one is $[1,2,4,3]$.</p>
