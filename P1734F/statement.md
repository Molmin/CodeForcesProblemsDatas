## Description

<div><p>Let $S$ be the <a href="https://en.wikipedia.org/wiki/Thue-Morse_sequence">Thue-Morse sequence</a>. In other words, $S$ is the $0$-indexed binary string with infinite length that can be constructed as follows: </p><ul> <li> Initially, let $S$ be "<span class="tex-font-style-tt">0</span>". </li><li> Then, we perform the following operation infinitely many times: concatenate $S$ with a copy of itself with flipped bits.<p>For example, here are the first four iterations: </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">Iteration</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$S$ before iteration</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$S$ before iteration with flipped bits</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">Concatenated $S$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top">1</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top"><span class="tex-font-style-tt">0</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top"><span class="tex-font-style-tt">1</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-top"><span class="tex-font-style-tt">01</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">2</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right"><span class="tex-font-style-tt">01</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right"><span class="tex-font-style-tt">10</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right"><span class="tex-font-style-tt">0110</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">3</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right"><span class="tex-font-style-tt">0110</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right"><span class="tex-font-style-tt">1001</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right"><span class="tex-font-style-tt">01101001</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">4</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right"><span class="tex-font-style-tt">01101001</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right"><span class="tex-font-style-tt">10010110</span></td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right"><span class="tex-font-style-tt">0110100110010110</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">$\ldots$</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-bottom">$\ldots$</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-bottom">$\ldots$</td><td class="tex-tabular-border-left tex-tabular-text-align-left tex-tabular-border-right tex-tabular-border-bottom">$\ldots$</td></tr></tbody></table> </center> </li></ul><p>You are given two positive integers $n$ and $m$. Find the number of positions where the strings $S_0 S_1 \ldots S_{m-1}$ and $S_n S_{n + 1} \ldots S_{n + m - 1}$ are different. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of the input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first and only line of each test case contains two positive integers, $n$ and $m$ respectively ($1 \leq n,m \leq 10^{18}$).</p></div><div class="output-specification"><p>For each testcase, output a non-negative integer&nbsp;— the Hamming distance between the two required strings.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of the input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first and only line of each test case contains two positive integers, $n$ and $m$ respectively ($1 \leq n,m \leq 10^{18}$).</p>

## Output

<p>For each testcase, output a non-negative integer&nbsp;— the Hamming distance between the two required strings.</p>





```input1|2,4,6
6
1 1
5 10
34 211
73 34
19124639 56348772
12073412269 96221437021
```




```output1
1
6
95
20
28208137
48102976088
```



## Note

<p>The string $S$ is equal to <span class="tex-font-style-tt">0110100110010110</span>....</p><p>In the first test case, $S_0$ is "<span class="tex-font-style-tt">0</span>", and $S_1$ is "<span class="tex-font-style-tt">1</span>". The Hamming distance between the two strings is $1$.</p><p>In the second test case, $S_0 S_1 \ldots S_9$ is "<span class="tex-font-style-tt">0110100110</span>", and $S_5 S_6 \ldots S_{14}$ is "<span class="tex-font-style-tt">0011001011</span>". The Hamming distance between the two strings is $6$.</p>
