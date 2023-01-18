## Description

<div><p>Mrs. Smith is trying to contact her husband, John Smith, but she forgot the secret phone number!</p><p>The only thing Mrs. Smith remembered was that any permutation of $n$ can be a secret phone number. Only those permutations that minimize secret value might be the phone of her husband.</p><p>The sequence of $n$ integers is called a permutation if it contains all integers from $1$ to $n$ exactly once.</p><p>The secret value of a phone number is defined as the sum of the length of the longest increasing subsequence (<span class="tex-font-style-tt">LIS</span>) and length of the longest decreasing subsequence (<span class="tex-font-style-tt">LDS</span>). </p><p>A subsequence $a_{i_1}, a_{i_2}, \ldots, a_{i_k}$ where $1\leq i_1 &lt; i_2 &lt; \ldots &lt; i_k\leq n$ is called increasing if $a_{i_1} &lt; a_{i_2} &lt; a_{i_3} &lt; \ldots &lt; a_{i_k}$. If $a_{i_1} &gt; a_{i_2} &gt; a_{i_3} &gt; \ldots &gt; a_{i_k}$, a subsequence is called decreasing. An increasing/decreasing subsequence is called longest if it has maximum length among all increasing/decreasing subsequences.</p><p>For example, if there is a permutation $[6, 4, 1, 7, 2, 3, 5]$, <span class="tex-font-style-tt">LIS</span> of this permutation will be $[1, 2, 3, 5]$, so the length of <span class="tex-font-style-tt">LIS</span> is equal to $4$. <span class="tex-font-style-tt">LDS</span> can be $[6, 4, 1]$, $[6, 4, 2]$, or $[6, 4, 3]$, so the length of <span class="tex-font-style-tt">LDS</span> is $3$.</p><p>Note, the lengths of <span class="tex-font-style-tt">LIS</span> and <span class="tex-font-style-tt">LDS</span> can be different.</p><p>So please help Mrs. Smith to find a permutation that gives a minimum sum of lengths of <span class="tex-font-style-tt">LIS</span> and <span class="tex-font-style-tt">LDS</span>.</p></div><div class="input-specification"><p>The only line contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of permutation that you need to build.</p></div><div class="output-specification"><p>Print a permutation that gives a minimum sum of lengths of <span class="tex-font-style-tt">LIS</span> and <span class="tex-font-style-tt">LDS</span>. </p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The only line contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of permutation that you need to build.</p>

## Output

<p>Print a permutation that gives a minimum sum of lengths of <span class="tex-font-style-tt">LIS</span> and <span class="tex-font-style-tt">LDS</span>. </p><p>If there are multiple answers, print any.</p>





```input1
4

```




```input2
2

```




```output1
3 4 1 2

```




```output2
2 1

```



## Note

<p>In the first sample, you can build a permutation $[3, 4, 1, 2]$. <span class="tex-font-style-tt">LIS</span> is $[3, 4]$ (or $[1, 2]$), so the length of <span class="tex-font-style-tt">LIS</span> is equal to $2$. <span class="tex-font-style-tt">LDS</span> can be ony of $[3, 1]$, $[4, 2]$, $[3, 2]$, or $[4, 1]$. The length of <span class="tex-font-style-tt">LDS</span> is also equal to $2$. The sum is equal to $4$. Note that $[3, 4, 1, 2]$ is <span class="tex-font-style-bf">not</span> the only permutation that is valid.</p><p>In the second sample, you can build a permutation $[2, 1]$. <span class="tex-font-style-tt">LIS</span> is $[1]$ (or $[2]$), so the length of <span class="tex-font-style-tt">LIS</span> is equal to $1$. <span class="tex-font-style-tt">LDS</span> is $[2, 1]$, so the length of <span class="tex-font-style-tt">LDS</span> is equal to $2$. The sum is equal to $3$. Note that permutation $[1, 2]$ is also valid.</p>
