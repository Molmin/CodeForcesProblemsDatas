## Description

<div><p>Let's define the <span class="tex-font-style-it">cost</span> of a string $s$ as the number of index pairs $i$ and $j$ ($1 \le i &lt; j &lt; |s|$) such that $s_i = s_j$ and $s_{i+1} = s_{j+1}$.</p><p>You are given two positive integers $n$ and $k$. Among all strings with length $n$ that contain only the first $k$ characters of the Latin alphabet, find a string with minimum possible <span class="tex-font-style-it">cost</span>. If there are multiple such strings with minimum <span class="tex-font-style-it">cost</span> — find any of them.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5; 1 \le k \le 26$).</p></div><div class="output-specification"><p>Print the string $s$ such that it consists of $n$ characters, each its character is one of the $k$ first Latin letters, and it has the minimum possible <span class="tex-font-style-it">cost</span> among all these strings. If there are multiple such strings — print any of them.</p></div>

## Input

<p>The only line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5; 1 \le k \le 26$).</p>

## Output

<p>Print the string $s$ such that it consists of $n$ characters, each its character is one of the $k$ first Latin letters, and it has the minimum possible <span class="tex-font-style-it">cost</span> among all these strings. If there are multiple such strings — print any of them.</p>





```input1
9 4
```




```input2
5 1
```




```input3
10 26
```




```output1
aabacadbb
```




```output2
aaaaa
```




```output3
codeforces
```


