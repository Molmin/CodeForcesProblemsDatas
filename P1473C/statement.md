## Description

<div><p>You have a sequence $a$ with $n$ elements $1, 2, 3, \dots, k - 1, k, k - 1, k - 2, \dots, k - (n - k)$ ($k \le n &lt; 2k$).</p><p>Let's call as inversion in $a$ a pair of indices $i &lt; j$ such that $a[i] &gt; a[j]$.</p><p>Suppose, you have some permutation $p$ of size $k$ and you build a sequence $b$ of size $n$ in the following manner: $b[i] = p[a[i]]$.</p><p>Your goal is to find such permutation $p$ that the total number of inversions in $b$ doesn't exceed the total number of inversions in $a$, and $b$ is <span class="tex-font-style-it">lexicographically maximum</span>.</p><p>Small reminder: the sequence of $k$ integers is called a permutation if it contains all integers from $1$ to $k$ exactly once.</p><p>Another small reminder: a sequence $s$ is <span class="tex-font-style-it">lexicographically smaller</span> than another sequence $t$, if either $s$ is a prefix of $t$, or for the first $i$ such that $s_i \ne t_i$, $s_i &lt; t_i$ holds (in the first position that these sequences are different, $s$ has smaller number than $t$).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $n$ and $k$ ($k \le n &lt; 2k$; $1 \le k \le 10^5$)&nbsp;— the length of the sequence $a$ and its maximum.</p><p>It's guaranteed that the total sum of $k$ over test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print $k$ integers&nbsp;— the permutation $p$ which maximizes $b$ lexicographically without increasing the total number of inversions.</p><p>It can be proven that $p$ exists and is unique.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $n$ and $k$ ($k \le n &lt; 2k$; $1 \le k \le 10^5$)&nbsp;— the length of the sequence $a$ and its maximum.</p><p>It's guaranteed that the total sum of $k$ over test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print $k$ integers&nbsp;— the permutation $p$ which maximizes $b$ lexicographically without increasing the total number of inversions.</p><p>It can be proven that $p$ exists and is unique.</p>





```input1
4
1 1
2 2
3 2
4 3
```




```output1
1 
1 2 
2 1 
1 3 2
```



## Note

<p>In the first test case, the sequence $a = [1]$, there is only one permutation $p = [1]$.</p><p>In the second test case, the sequence $a = [1, 2]$. There is no inversion in $a$, so there is only one permutation $p = [1, 2]$ which doesn't increase the number of inversions.</p><p>In the third test case, $a = [1, 2, 1]$ and has $1$ inversion. If we use $p = [2, 1]$, then $b = [p[a[1]], p[a[2]], p[a[3]]] = [2, 1, 2]$ and also has $1$ inversion.</p><p>In the fourth test case, $a = [1, 2, 3, 2]$, and since $p = [1, 3, 2]$ then $b = [1, 3, 2, 3]$. Both $a$ and $b$ have $1$ inversion and $b$ is the lexicographically maximum.</p>
