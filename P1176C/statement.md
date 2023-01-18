## Description

<div><p>You are given an array $a$ consisting of $n$ integers. Each $a_i$ is one of the six following numbers: $4, 8, 15, 16, 23, 42$.</p><p>Your task is to remove the minimum number of elements to make this array <span class="tex-font-style-bf">good</span>.</p><p>An array of length $k$ is called <span class="tex-font-style-bf">good</span> if $k$ is divisible by $6$ and it is possible to split it into $\frac{k}{6}$ <span class="tex-font-style-bf">subsequences</span> $4, 8, 15, 16, 23, 42$.</p><p>Examples of good arrays:</p><ul> <li> $[4, 8, 15, 16, 23, 42]$ (the whole array is a required sequence); </li><li> $[4, 8, 4, 15, 16, 8, 23, 15, 16, 42, 23, 42]$ (the first sequence is formed from first, second, fourth, fifth, seventh and tenth elements and the second one is formed from remaining elements); </li><li> $[]$ (<span class="tex-font-style-bf">the empty array is good</span>). </li></ul><p>Examples of bad arrays: </p><ul> <li> $[4, 8, 15, 16, 42, 23]$ (the order of elements should be exactly $4, 8, 15, 16, 23, 42$); </li><li> $[4, 8, 15, 16, 23, 42, 4]$ (the length of the array is not divisible by $6$); </li><li> $[4, 8, 15, 16, 23, 42, 4, 8, 15, 16, 23, 23]$ (the first sequence can be formed from first six elements but the remaining array cannot form the required sequence). </li></ul></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ (each $a_i$ is one of the following numbers: $4, 8, 15, 16, 23, 42$), where $a_i$ is the $i$-th element of $a$.</p></div><div class="output-specification"><p>Print one integer — the minimum number of elements you have to remove to obtain a <span class="tex-font-style-bf">good</span> array.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ (each $a_i$ is one of the following numbers: $4, 8, 15, 16, 23, 42$), where $a_i$ is the $i$-th element of $a$.</p>

## Output

<p>Print one integer — the minimum number of elements you have to remove to obtain a <span class="tex-font-style-bf">good</span> array.</p>





```input1
5
4 8 15 16 23
```




```input2
12
4 8 4 15 16 8 23 15 16 42 23 42
```




```input3
15
4 8 4 8 15 16 8 16 23 15 16 4 42 23 42
```




```output1
5
```




```output2
0
```




```output3
3
```


