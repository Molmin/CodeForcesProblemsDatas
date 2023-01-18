## Description

<div><p>The Fair Nut has two arrays $a$ and $b$, consisting of $n$ numbers. He found them so long ago that no one knows when they came to him.</p><p>The Fair Nut often changes numbers in his arrays. He also is interested in how similar $a$ and $b$ are after every modification.</p><p>Let's denote similarity of two arrays as the minimum number of operations to apply to make arrays equal (every operation can be applied for both arrays). If it is impossible, similarity will be equal $-1$.</p><p>Per one operation you can choose a subarray with length $k$ ($k$ is fixed), and change every element $a_i$, which belongs to the chosen subarray, to $a_i \oplus x$ ($x$ can be chosen), where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. </p><p>Nut has already calculated the similarity of the arrays after every modification. Can you do it?</p><p>Note that you just need to calculate those values, that is you do not need to apply any operations.</p></div><div class="input-specification"><p>The first line contains three numbers $n$, $k$ and $q$ ($1 \le k \le n \le 2 \cdot 10^5$, $0 \le q \le 2 \cdot 10^5$)&nbsp;— the length of the arrays, the length of the subarrays, to which the operations are applied, and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{14}$)&nbsp;— elements of array $a$.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \le b_i &lt; 2^{14}$)&nbsp;— elements of array $b$.</p><p>Each of the next $q$ lines describes query and contains string $s$ and two integers $p$ and $v$ ($1 \le p \le n$, $0 \le v &lt; 2^{14}$)&nbsp;— array, which this query changes («<span class="tex-font-style-tt">a</span>» or «<span class="tex-font-style-tt">b</span>» without quotes), index of changing element and its new value.</p></div><div class="output-specification"><p>On the first line print initial similarity of arrays $a$ and $b$.</p><p>On the $i$-th of following $q$ lines print similarity of $a$ and $b$ after applying first $i$ modifications.</p></div>

## Input

<p>The first line contains three numbers $n$, $k$ and $q$ ($1 \le k \le n \le 2 \cdot 10^5$, $0 \le q \le 2 \cdot 10^5$)&nbsp;— the length of the arrays, the length of the subarrays, to which the operations are applied, and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{14}$)&nbsp;— elements of array $a$.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \le b_i &lt; 2^{14}$)&nbsp;— elements of array $b$.</p><p>Each of the next $q$ lines describes query and contains string $s$ and two integers $p$ and $v$ ($1 \le p \le n$, $0 \le v &lt; 2^{14}$)&nbsp;— array, which this query changes («<span class="tex-font-style-tt">a</span>» or «<span class="tex-font-style-tt">b</span>» without quotes), index of changing element and its new value.</p>

## Output

<p>On the first line print initial similarity of arrays $a$ and $b$.</p><p>On the $i$-th of following $q$ lines print similarity of $a$ and $b$ after applying first $i$ modifications.</p>





```input1
3 3 1
0 4 2
1 2 3
b 2 5

```




```input2
3 2 2
1 3 2
0 0 0
a 1 0
b 1 1

```




```output1
-1
1

```




```output2
2
-1
2

```



## Note

<p>In the first sample making arrays $[0, 4, 2]$ and $[1, 2, 3]$ is impossible with $k=3$. After the modification, you can apply the operation with $x=1$ to the whole first array (its length is equal to $k$), and it will be equal to the second array.</p><p>In order to make arrays equal in the second sample before changes, you can apply operations with $x=1$ on subarray $[1, 2]$ of $a$ and with $x=2$ on subarray $[2, 3]$ of $b$.</p><p>After all queries arrays will be equal $[0, 3, 2]$ and $[1, 0, 0]$. The same operations make them equal $[1, 2, 2]$.</p>
