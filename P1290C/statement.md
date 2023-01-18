## Description

<div><p>There are $n$ lamps on a line, numbered from $1$ to $n$. Each one has an initial state off ($0$) or on ($1$).</p><p>You're given $k$ subsets $A_1, \ldots, A_k$ of $\{1, 2, \dots, n\}$, such that the intersection of any three subsets is empty. In other words, for all $1 \le i_1 &lt; i_2 &lt; i_3 \le k$, $A_{i_1} \cap A_{i_2} \cap A_{i_3} = \varnothing$.</p><p>In one operation, you can choose one of these $k$ subsets and switch the state of all lamps in it. It is guaranteed that, with the given subsets, it's possible to make all lamps be simultaneously on using this type of operation.</p><p>Let $m_i$ be the minimum number of operations you have to do in order to make the $i$ first lamps be simultaneously on. Note that there is no condition upon the state of other lamps (between $i+1$ and $n$), they can be either off or on.</p><p>You have to compute $m_i$ for all $1 \le i \le n$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n, k \le 3 \cdot 10^5$).</p><p>The second line contains a binary string of length $n$, representing the initial state of each lamp (the lamp $i$ is off if $s_i = 0$, on if $s_i = 1$).</p><p>The description of each one of the $k$ subsets follows, in the following format:</p><p>The first line of the description contains a single integer $c$ ($1 \le c \le n$) &nbsp;— the number of elements in the subset.</p><p>The second line of the description contains $c$ distinct integers $x_1, \ldots, x_c$ ($1 \le x_i \le n$) &nbsp;— the elements of the subset.</p><p>It is guaranteed that: </p><ul> <li> The intersection of any three subsets is empty; </li><li> It's possible to make all lamps be simultaneously on using some operations. </li></ul></div><div class="output-specification"><p>You must output $n$ lines. The $i$-th line should contain a single integer $m_i$ &nbsp;— the minimum number of operations required to make the lamps $1$ to $i$ be simultaneously on.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n, k \le 3 \cdot 10^5$).</p><p>The second line contains a binary string of length $n$, representing the initial state of each lamp (the lamp $i$ is off if $s_i = 0$, on if $s_i = 1$).</p><p>The description of each one of the $k$ subsets follows, in the following format:</p><p>The first line of the description contains a single integer $c$ ($1 \le c \le n$) &nbsp;— the number of elements in the subset.</p><p>The second line of the description contains $c$ distinct integers $x_1, \ldots, x_c$ ($1 \le x_i \le n$) &nbsp;— the elements of the subset.</p><p>It is guaranteed that: </p><ul> <li> The intersection of any three subsets is empty; </li><li> It's possible to make all lamps be simultaneously on using some operations. </li></ul>

## Output

<p>You must output $n$ lines. The $i$-th line should contain a single integer $m_i$ &nbsp;— the minimum number of operations required to make the lamps $1$ to $i$ be simultaneously on.</p>





```input1
7 3
0011100
3
1 4 6
3
3 4 7
2
2 3
```




```input2
8 6
00110011
3
1 3 8
5
1 2 5 6 7
2
6 8
2
3 5
2
4 7
1
2
```




```input3
5 3
00011
3
1 2 3
1
4
3
3 4 5
```




```input4
19 5
1001001001100000110
2
2 3
2
5 6
2
8 9
5
12 13 14 15 16
1
19
```




```output1
1
2
3
3
3
3
3
```




```output2
1
1
1
1
1
1
4
4
```




```output3
1
1
1
1
1
```




```output4
0
1
1
1
2
2
2
3
3
3
3
4
4
4
4
4
4
4
5
```



## Note

<p>In the first example: </p><ul> <li> For $i = 1$, we can just apply one operation on $A_1$, the final states will be $1010110$; </li><li> For $i = 2$, we can apply operations on $A_1$ and $A_3$, the final states will be $1100110$; </li><li> For $i \ge 3$, we can apply operations on $A_1$, $A_2$ and $A_3$, the final states will be $1111111$. </li></ul><p>In the second example: </p><ul> <li> For $i \le 6$, we can just apply one operation on $A_2$, the final states will be $11111101$; </li><li> For $i \ge 7$, we can apply operations on $A_1, A_3, A_4, A_6$, the final states will be $11111111$. </li></ul>
