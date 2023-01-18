## Description

<div><p>Word $s$ of length $n$ is called $k$-complete if </p><ul> <li> $s$ is a palindrome, i.e. $s_i=s_{n+1-i}$ for all $1 \le i \le n$; </li><li> $s$ has a period of $k$, i.e. $s_i=s_{k+i}$ for all $1 \le i \le n-k$. </li></ul><p>For example, "<span class="tex-font-style-tt">abaaba</span>" is a $3$-complete word, while "<span class="tex-font-style-tt">abccba</span>" is not.</p><p>Bob is given a word $s$ of length $n$ consisting of only lowercase Latin letters and an integer $k$, such that $n$ is divisible by $k$. He wants to convert $s$ to any $k$-complete word.</p><p>To do this Bob can choose some $i$ ($1 \le i \le n$) and replace the letter at position $i$ with some other lowercase Latin letter.</p><p>So now Bob wants to know the minimum number of letters he has to replace to convert $s$ to any $k$-complete word.</p><p>Note that Bob can do zero changes if the word $s$ is already $k$-complete.</p><p>You are required to answer $t$ test cases <span class="tex-font-style-bf">independently</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t\le 10^5$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k &lt; n \le 2 \cdot 10^5$, $n$ is divisible by $k$).</p><p>The second line of each test case contains a word $s$ of length $n$.</p><p>It is guaranteed that word $s$ only contains lowercase Latin letters. And it is guaranteed that the sum of $n$ over all test cases will not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output one integer, representing the minimum number of characters he has to replace to convert $s$ to any $k$-complete word.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t\le 10^5$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k &lt; n \le 2 \cdot 10^5$, $n$ is divisible by $k$).</p><p>The second line of each test case contains a word $s$ of length $n$.</p><p>It is guaranteed that word $s$ only contains lowercase Latin letters. And it is guaranteed that the sum of $n$ over all test cases will not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output one integer, representing the minimum number of characters he has to replace to convert $s$ to any $k$-complete word.</p>





```input1
4
6 2
abaaba
6 3
abaaba
36 9
hippopotomonstrosesquippedaliophobia
21 7
wudixiaoxingxingheclp
```




```output1
2
0
23
16
```



## Note

<p>In the first test case, one optimal solution is <span class="tex-font-style-tt">a<span class="tex-font-style-underline"><span class="tex-font-style-bf">a</span></span>aa<span class="tex-font-style-underline"><span class="tex-font-style-bf">a</span></span>a</span>.</p><p>In the second test case, the given word itself is $k$-complete.</p>
