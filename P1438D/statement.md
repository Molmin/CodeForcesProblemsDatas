## Description

<div><p>Ksenia has an array $a$ consisting of $n$ positive integers $a_1, a_2, \ldots, a_n$. </p><p>In one operation she can do the following: </p><ul> <li> choose three distinct indices $i$, $j$, $k$, and then </li><li> change all of $a_i, a_j, a_k$ to $a_i \oplus a_j \oplus a_k$ simultaneously, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. </li></ul><p>She wants to make all $a_i$ equal <span class="tex-font-style-bf">in at most $n$ operations</span>, or to determine that it is impossible to do so. She wouldn't ask for your help, but please, help her!</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($3 \leq n \leq 10^5$)&nbsp;— the length of $a$.</p><p>The second line contains $n$ integers, $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— elements of $a$.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span> in the first line depending on whether it is possible to make all elements equal in at most $n$ operations.</p><p>If it is possible, print an integer $m$ ($0 \leq m \leq n$), which denotes the number of operations you do.</p><p>In each of the next $m$ lines, print three distinct integers $i, j, k$, representing one operation. </p><p>If there are many such operation sequences possible, print any. Note that you do <span class="tex-font-style-bf">not</span> have to minimize the number of operations.</p></div>

## Input

<p>The first line contains one integer $n$ ($3 \leq n \leq 10^5$)&nbsp;— the length of $a$.</p><p>The second line contains $n$ integers, $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— elements of $a$.</p>

## Output

<p>Print <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span> in the first line depending on whether it is possible to make all elements equal in at most $n$ operations.</p><p>If it is possible, print an integer $m$ ($0 \leq m \leq n$), which denotes the number of operations you do.</p><p>In each of the next $m$ lines, print three distinct integers $i, j, k$, representing one operation. </p><p>If there are many such operation sequences possible, print any. Note that you do <span class="tex-font-style-bf">not</span> have to minimize the number of operations.</p>





```input1
5
4 2 1 7 2
```




```input2
4
10 4 49 22
```




```output1
YES
1
1 3 4
```




```output2
NO
```



## Note

<p>In the first example, the array becomes $[4 \oplus 1 \oplus 7, 2, 4 \oplus 1 \oplus 7, 4 \oplus 1 \oplus 7, 2] = [2, 2, 2, 2, 2]$.</p>
