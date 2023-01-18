## Description

<div><p>You are given a ternary string (it is a string which consists only of characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">2</span>').</p><p>You can swap any two adjacent (consecutive) characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' (i.e. replace "<span class="tex-font-style-tt">01</span>" with "<span class="tex-font-style-tt">10</span>" or vice versa) or any two adjacent (consecutive) characters '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">2</span>' (i.e. replace "<span class="tex-font-style-tt">12</span>" with "<span class="tex-font-style-tt">21</span>" or vice versa).</p><p>For example, for string "<span class="tex-font-style-tt">010210</span>" we can perform the following moves: </p><ul> <li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline">01</span>0210</span>" $\rightarrow$ "<span class="tex-font-style-tt"><span class="tex-font-style-underline">10</span>0210</span>"; </li><li> "<span class="tex-font-style-tt">0<span class="tex-font-style-underline">10</span>210</span>" $\rightarrow$ "<span class="tex-font-style-tt">0<span class="tex-font-style-underline">01</span>210</span>"; </li><li> "<span class="tex-font-style-tt">010<span class="tex-font-style-underline">21</span>0</span>" $\rightarrow$ "<span class="tex-font-style-tt">010<span class="tex-font-style-underline">12</span>0</span>"; </li><li> "<span class="tex-font-style-tt">0102<span class="tex-font-style-underline">10</span></span>" $\rightarrow$ "<span class="tex-font-style-tt">0102<span class="tex-font-style-underline">01</span></span>". </li></ul><p>Note than you cannot swap "<span class="tex-font-style-tt"><span class="tex-font-style-underline">02</span></span>" $\rightarrow$ "<span class="tex-font-style-tt"><span class="tex-font-style-underline">20</span></span>" and vice versa. You cannot perform any other operations with the given string excluding described above.</p><p>You task is to obtain the minimum possible (lexicographically) string by using these swaps arbitrary number of times (<span class="tex-font-style-it">possibly, zero</span>).</p><p>String $a$ is lexicographically less than string $b$ (if strings $a$ and $b$ have the same length) if there exists some position $i$ ($1 \le i \le |a|$, where $|s|$ is the length of the string $s$) such that for every $j &lt; i$ holds $a_j = b_j$, and $a_i &lt; b_i$.</p></div><div class="input-specification"><p>The first line of the input contains the string $s$ consisting only of characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">2</span>', its length is between $1$ and $10^5$ (inclusive).</p></div><div class="output-specification"><p>Print a single string — the minimum possible (lexicographically) string you can obtain by using the swaps described above arbitrary number of times (<span class="tex-font-style-it">possibly, zero</span>).</p></div>

## Input

<p>The first line of the input contains the string $s$ consisting only of characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">2</span>', its length is between $1$ and $10^5$ (inclusive).</p>

## Output

<p>Print a single string — the minimum possible (lexicographically) string you can obtain by using the swaps described above arbitrary number of times (<span class="tex-font-style-it">possibly, zero</span>).</p>





```input1
100210

```




```input2
11222121

```




```input3
20

```




```output1
001120

```




```output2
11112222

```




```output3
20

```


