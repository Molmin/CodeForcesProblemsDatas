## Description

<div><center> <img class="tex-graphics" height="302px" src="file://mVXanziy.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>William has two arrays $a$ and $b$, each consisting of $n$ items.</p><p>For some segments $l..r$ of these arrays William wants to know if it is possible to equalize the values of items in these segments using a balancing operation. Formally, the values are equalized if for each $i$ from $l$ to $r$ holds $a_i = b_i$.</p><p>To perform a balancing operation an even number of indices must be selected, such that $l \le pos_1 &lt; pos_2 &lt; \dots &lt; pos_k \le r$. Next the items of <span class="tex-font-style-bf">array a</span> at positions $pos_1, pos_3, pos_5, \dots$ get incremented by one and the items of <span class="tex-font-style-bf">array b</span> at positions $pos_2, pos_4, pos_6, \dots$ get incremented by one.</p><p>William wants to find out if it is possible to equalize the values of elements in two arrays for each segment using some number of balancing operations, and what is the minimal number of operations required for that. Note that for each segment the operations are performed independently.</p></div><div class="input-specification"><p>The first line contains a two integers $n$ and $q$ ($2 \le n \le 10^5$, $1 \le q \le 10^5$), the size of arrays $a$ and $b$ and the number of segments.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(0 \le a_i \le 10^9)$.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ $(0 \le b_i \le 10^9)$.</p><p>Each of the next $q$ lines contains two integers $l_i$ and $r_i$ $(1 \le l_i &lt; r_i \le n)$, the edges of segments.</p></div><div class="output-specification"><p>For each segment output a single number&nbsp;— the minimal number of balancing operations needed or "<span class="tex-font-style-tt">-1</span>" if it is impossible to equalize segments of arrays.</p></div>

## Input

<p>The first line contains a two integers $n$ and $q$ ($2 \le n \le 10^5$, $1 \le q \le 10^5$), the size of arrays $a$ and $b$ and the number of segments.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(0 \le a_i \le 10^9)$.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ $(0 \le b_i \le 10^9)$.</p><p>Each of the next $q$ lines contains two integers $l_i$ and $r_i$ $(1 \le l_i &lt; r_i \le n)$, the edges of segments.</p>

## Output

<p>For each segment output a single number&nbsp;— the minimal number of balancing operations needed or "<span class="tex-font-style-tt">-1</span>" if it is impossible to equalize segments of arrays.</p>





```input1
8 5
0 1 2 9 3 2 7 5
2 2 1 9 4 1 5 8
2 6
1 7
2 4
7 8
5 8
```




```output1
1
3
1
-1
-1
```



## Note

<p>For the first segment from $2$ to $6$ you can do one operation with $pos = [2, 3, 5, 6]$, after this operation the arrays will be: $a = [0, 2, 2, 9, 4, 2, 7, 5]$, $b = [2, 2, 2, 9, 4, 2, 5, 8]$. Arrays are equal on a segment from $2$ to $6$ after this operation.</p><p>For the second segment from $1$ to $7$ you can do three following operations: </p><ol> <li> $pos = [1, 3, 5, 6]$ </li><li> $pos = [1, 7]$ </li><li> $pos = [2, 7]$ </li></ol><p>After these operations, the arrays will be: $a = [2, 2, 2, 9, 4, 2, 7, 5]$, $b = [2, 2, 2, 9, 4, 2, 7, 8]$. Arrays are equal on a segment from $1$ to $7$ after these operations.</p><p>For the third segment from $2$ to $4$ you can do one operation with $pos = [2, 3]$, after the operation arrays will be: $a = [0, 2, 2, 9, 3, 2, 7, 5]$, $b = [2, 2, 2, 9, 4, 1, 5, 8]$. Arrays are equal on a segment from $2$ to $4$ after this operation.</p><p>It is impossible to equalize the fourth and the fifth segment.</p>
