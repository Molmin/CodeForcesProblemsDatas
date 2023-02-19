## Description

<div><p>Suppose you have an integer $v$. In one operation, you can: </p><ul> <li> either set $v = (v + 1) \bmod 32768$ </li><li> or set $v = (2 \cdot v) \bmod 32768$. </li></ul><p>You are given $n$ integers $a_1, a_2, \dots, a_n$. What is the minimum number of operations you need to make each $a_i$ equal to $0$?</p></div><div class="input-specification"><p>The first line contains the single integer $n$ ($1 \le n \le 32768$)&nbsp;— the number of integers.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i &lt; 32768$).</p></div><div class="output-specification"><p>Print $n$ integers. The $i$-th integer should be equal to the minimum number of operations required to make $a_i$ equal to $0$.</p></div>

## Input

<p>The first line contains the single integer $n$ ($1 \le n \le 32768$)&nbsp;— the number of integers.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i &lt; 32768$).</p>

## Output

<p>Print $n$ integers. The $i$-th integer should be equal to the minimum number of operations required to make $a_i$ equal to $0$.</p>





```input1
4
19 32764 10240 49
```




```output1
14 4 4 15
```



## Note

<p>Let's consider each $a_i$: </p><ul> <li> $a_1 = 19$. You can, firstly, increase it by one to get $20$ and then multiply it by two $13$ times. You'll get $0$ in $1 + 13 = 14$ steps. </li><li> $a_2 = 32764$. You can increase it by one $4$ times: $32764 \rightarrow 32765 \rightarrow 32766 \rightarrow 32767 \rightarrow 0$. </li><li> $a_3 = 10240$. You can multiply it by two $4$ times: $10240 \rightarrow 20480 \rightarrow 8192 \rightarrow 16384 \rightarrow 0$. </li><li> $a_4 = 49$. You can multiply it by two $15$ times. </li></ul>
