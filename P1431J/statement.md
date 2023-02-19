## Description

<div><p>You are given an array of integers $a$ of size $n$. This array is non-decreasing, i. e. $a_1 \le a_2 \le \dots \le a_n$.</p><p>You have to find arrays of integers $b$ of size $2n - 1$, such that:</p><ul> <li> $b_{2i-1} = a_i$ ($1 \le i \le n$); </li><li> array $b$ is non-decreasing; </li><li> $b_1 \oplus b_2 \oplus \dots \oplus b_{2n-1} = 0$ ($\oplus$ denotes bitwise XOR operation: <a href="https://en.wikipedia.org/wiki/Exclusive_or">https://en.wikipedia.org/wiki/Exclusive_or</a>. In Kotlin, it is <span class="tex-font-style-tt">xor</span> function). </li></ul><p>Calculate the number of arrays that meet all the above conditions, modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 17$) — the size of the array $a$.</p><p>The second line contains $n$ integers ($0 \le a_i \le 2^{60} - 1; a_i \le a_{i+1}$) — elements of the array $a$.</p></div><div class="output-specification"><p>Print a single integer — the number of arrays that meet all the above conditions, modulo $998244353$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 17$) — the size of the array $a$.</p><p>The second line contains $n$ integers ($0 \le a_i \le 2^{60} - 1; a_i \le a_{i+1}$) — elements of the array $a$.</p>

## Output

<p>Print a single integer — the number of arrays that meet all the above conditions, modulo $998244353$.</p>





```input1
3
0 1 3
```




```input2
4
0 3 6 7
```




```input3
5
1 5 9 10 23
```




```input4
10
39 62 64 79 81 83 96 109 120 122
```




```output1
2
```




```output2
6
```




```output3
20
```




```output4
678132
```


