## Description

<div><p>Given a permutation $p$ of length $n$, find its subsequence $s_1$, $s_2$, $\ldots$, $s_k$ of length at least $2$ such that:</p><ul> <li> $|s_1-s_2|+|s_2-s_3|+\ldots+|s_{k-1}-s_k|$ is as big as possible over all subsequences of $p$ with length at least $2$. </li><li> Among all such subsequences, choose the one whose length, $k$, is as small as possible. </li></ul><p>If multiple subsequences satisfy these conditions, you are allowed to find any of them.</p><p>A sequence $a$ is a subsequence of an array $b$ if $a$ can be obtained from $b$ by deleting some (possibly, zero or all) elements.</p><p>A permutation of length $n$ is an array of length $n$ in which every element from $1$ to $n$ occurs exactly once.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 2 \cdot 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 10^5$)&nbsp;— the length of the permutation $p$.</p><p>The second line of each test case contains $n$ integers $p_1$, $p_2$, $\ldots$, $p_{n}$ ($1 \le p_i \le n$, $p_i$ are distinct)&nbsp;— the elements of the permutation $p$.</p><p><span class="tex-font-style-bf">The sum of $n$ across the test cases doesn't exceed $10^5$.</span></p></div><div class="output-specification"><p>For each test case, the first line should contain the length of the found subsequence, $k$. The second line should contain $s_1$, $s_2$, $\ldots$, $s_k$&nbsp;— its elements.</p><p>If multiple subsequences satisfy these conditions, you are allowed to find any of them.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 2 \cdot 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 10^5$)&nbsp;— the length of the permutation $p$.</p><p>The second line of each test case contains $n$ integers $p_1$, $p_2$, $\ldots$, $p_{n}$ ($1 \le p_i \le n$, $p_i$ are distinct)&nbsp;— the elements of the permutation $p$.</p><p><span class="tex-font-style-bf">The sum of $n$ across the test cases doesn't exceed $10^5$.</span></p>

## Output

<p>For each test case, the first line should contain the length of the found subsequence, $k$. The second line should contain $s_1$, $s_2$, $\ldots$, $s_k$&nbsp;— its elements.</p><p>If multiple subsequences satisfy these conditions, you are allowed to find any of them.</p>





```input1
2
3
3 2 1
4
1 3 4 2
```




```output1
2
3 1 
3
1 4 2
```



## Note

<p>In the first test case, there are $4$ subsequences of length at least $2$:</p><ul> <li> $[3,2]$ which gives us $|3-2|=1$. </li><li> $[3,1]$ which gives us $|3-1|=2$. </li><li> $[2,1]$ which gives us $|2-1|=1$. </li><li> $[3,2,1]$ which gives us $|3-2|+|2-1|=2$. </li></ul><p>So the answer is either $[3,1]$ or $[3,2,1]$. Since we want the subsequence to be as short as possible, the answer is $[3,1]$.</p>
