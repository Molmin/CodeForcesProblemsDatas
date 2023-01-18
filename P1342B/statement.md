## Description

<div><p>Let's say string $s$ has period $k$ if $s_i = s_{i + k}$ for all $i$ from $1$ to $|s| - k$ ($|s|$ means length of string $s$) and $k$ is the minimum positive integer with this property.</p><p>Some examples of a period: for $s$="<span class="tex-font-style-tt">0101</span>" the period is $k=2$, for $s$="<span class="tex-font-style-tt">0000</span>" the period is $k=1$, for $s$="<span class="tex-font-style-tt">010</span>" the period is $k=2$, for $s$="<span class="tex-font-style-tt">0011</span>" the period is $k=4$.</p><p>You are given string $t$ consisting only of <span class="tex-font-style-tt">0</span>'s and <span class="tex-font-style-tt">1</span>'s and you need to find such string $s$ that:</p><ol> <li> String $s$ consists only of <span class="tex-font-style-tt">0</span>'s and <span class="tex-font-style-tt">1</span>'s; </li><li> The length of $s$ doesn't exceed $2 \cdot |t|$; </li><li> String $t$ is a subsequence of string $s$; </li><li> String $s$ has smallest possible period among all strings that meet conditions 1—3. </li></ol><p>Let us recall that $t$ is a subsequence of $s$ if $t$ can be derived from $s$ by deleting zero or more elements (any) without changing the order of the remaining elements. For example, $t$="<span class="tex-font-style-tt">011</span>" is a subsequence of $s$="<span class="tex-font-style-tt">10101</span>".</p></div><div class="input-specification"><p>The first line contains single integer $T$ ($1 \le T \le 100$)&nbsp;— the number of test cases.</p><p>Next $T$ lines contain test cases — one per line. Each line contains string $t$ ($1 \le |t| \le 100$) consisting only of <span class="tex-font-style-tt">0</span>'s and <span class="tex-font-style-tt">1</span>'s.</p></div><div class="output-specification"><p>Print one string for each test case — string $s$ you needed to find. If there are multiple solutions print any one of them.</p></div>

## Input

<p>The first line contains single integer $T$ ($1 \le T \le 100$)&nbsp;— the number of test cases.</p><p>Next $T$ lines contain test cases — one per line. Each line contains string $t$ ($1 \le |t| \le 100$) consisting only of <span class="tex-font-style-tt">0</span>'s and <span class="tex-font-style-tt">1</span>'s.</p>

## Output

<p>Print one string for each test case — string $s$ you needed to find. If there are multiple solutions print any one of them.</p>





```input1
4
00
01
111
110
```




```output1
00
01
11111
1010
```



## Note

<p>In the first and second test cases, $s = t$ since it's already one of the optimal solutions. Answers have periods equal to $1$ and $2$, respectively.</p><p>In the third test case, there are shorter optimal solutions, but it's okay since we don't need to minimize the string $s$. String $s$ has period equal to $1$.</p>
