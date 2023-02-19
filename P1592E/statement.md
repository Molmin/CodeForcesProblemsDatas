## Description

<div><p>Bakry got bored of solving problems related to xor, so he asked you to solve this problem for him.</p><p>You are given an array $a$ of $n$ integers $[a_1, a_2, \ldots, a_n]$.</p><p>Let's call a subarray $a_{l}, a_{l+1}, a_{l+2}, \ldots, a_r$ <span class="tex-font-style-bf">good</span> if $a_l \, \&amp; \, a_{l+1} \, \&amp; \, a_{l+2} \, \ldots \, \&amp; \, a_r &gt; a_l \oplus a_{l+1} \oplus a_{l+2} \ldots \oplus a_r$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a> and $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>.</p><p>Find the length of the longest good subarray of $a$, or determine that no such subarray exists.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^6$) — the length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$) — elements of the array.</p></div><div class="output-specification"><p>Print a single integer — the length of the longest good subarray. If there are no good subarrays, print $0$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^6$) — the length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$) — elements of the array.</p>

## Output

<p>Print a single integer — the length of the longest good subarray. If there are no good subarrays, print $0$.</p>





```input1
2
5 6
```




```input2
3
2 4 3
```




```input3
6
8 1 3 3 1 2
```




```output1
2
```




```output2
0
```




```output3
4
```



## Note

<p>In the first case, the answer is $2$, as the whole array is good: $5 \&amp; 6 = 4 &gt; 5 \oplus 6 = 3$.</p><p>In the third case, the answer is $4$, and one of the longest good subarrays is $[a_2, a_3, a_4, a_5]$: $1\&amp; 3 \&amp; 3 \&amp;1 = 1 &gt; 1\oplus 3 \oplus 3\oplus 1 = 0$.</p>
