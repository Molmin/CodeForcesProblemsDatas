## Description

<div><p>You have a binary string $a$ of length $n$ consisting only of digits $0$ and $1$. </p><p>You are given $q$ queries. In the $i$-th query, you are given two indices $l$ and $r$ such that $1 \le l \le r \le n$. </p><p>Let $s=a[l,r]$. You are allowed to do the following operation on $s$:</p><ol> <li> Choose two indices $x$ and $y$ such that $1 \le x \le y \le |s|$. Let $t$ be the substring $t = s[x, y]$. Then for all $1 \le i \le |t| - 1$, the condition $t_i \neq t_{i+1}$ has to hold. Note that $x = y$ is always a valid substring. </li><li> Delete the substring $s[x, y]$ from $s$. </li></ol><p>For each of the $q$ queries, find the minimum number of operations needed to make $s$ an empty string.</p><p>Note that for a string $s$, $s[l,r]$ denotes the subsegment $s_l,s_{l+1},\ldots,s_r$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10 ^ 5$) &nbsp;— the length of the binary string $a$ and the number of queries respectively.</p><p>The second line contains a binary string $a$ of length $n$ ($a_i \in \{0, 1\}$).</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le n$) &nbsp;— representing the substring of each query.</p></div><div class="output-specification"><p>Print $q$ lines, the $i$-th line representing the minimum number of operations needed for the $i$-th query.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10 ^ 5$) &nbsp;— the length of the binary string $a$ and the number of queries respectively.</p><p>The second line contains a binary string $a$ of length $n$ ($a_i \in \{0, 1\}$).</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le n$) &nbsp;— representing the substring of each query.</p>

## Output

<p>Print $q$ lines, the $i$-th line representing the minimum number of operations needed for the $i$-th query.</p>





```input1
5 3
11011
2 4
1 5
3 5
```




```input2
10 3
1001110110
1 10
2 5
5 10
```




```output1
1
3
2
```




```output2
4
2
3
```



## Note

<p>In the first test case, </p><ol> <li> The substring is $\texttt{101}$, so we can do one operation to make the substring empty. </li><li> The substring is $\texttt{11011}$, so we can do one operation on $s[2, 4]$ to make $\texttt{11}$, then use two more operations to make the substring empty. </li><li> The substring is $\texttt{011}$, so we can do one operation on $s[1, 2]$ to make $\texttt{1}$, then use one more operation to make the substring empty. </li></ol>
