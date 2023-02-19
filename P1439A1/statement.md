## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between the versions is in the number of possible operations that can be made. You can make hacks if and only if you solved both versions of the problem.</span></p><p>You are given a binary table of size $n \times m$. This table consists of symbols $0$ and $1$.</p><p>You can make such operation: select $3$ different cells that belong to one $2 \times 2$ square and change the symbols in these cells (change $0$ to $1$ and $1$ to $0$).</p><p>Your task is to make all symbols in the table equal to $0$. You are allowed to make at most $3nm$ operations. <span class="tex-font-style-bf">You don't need to minimize the number of operations.</span></p><p>It can be proved that it is always possible.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 5000$)&nbsp;— the number of test cases. The next lines contain descriptions of test cases.</p><p>The first line of the description of each test case contains two integers $n$, $m$ ($2 \leq n, m \leq 100$).</p><p>Each of the next $n$ lines contains a binary string of length $m$, describing the symbols of the next row of the table.</p><p>It is guaranteed that the sum of $nm$ for all test cases does not exceed $20000$.</p></div><div class="output-specification"><p>For each test case print the integer $k$ ($0 \leq k \leq 3nm$)&nbsp;— the number of operations.</p><p>In the each of the next $k$ lines print $6$ integers $x_1, y_1, x_2, y_2, x_3, y_3$ ($1 \leq x_1, x_2, x_3 \leq n, 1 \leq y_1, y_2, y_3 \leq m$) describing the next operation. This operation will be made with three cells $(x_1, y_1)$, $(x_2, y_2)$, $(x_3, y_3)$. These three cells should be different. These three cells should belong into some $2 \times 2$ square.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 5000$)&nbsp;— the number of test cases. The next lines contain descriptions of test cases.</p><p>The first line of the description of each test case contains two integers $n$, $m$ ($2 \leq n, m \leq 100$).</p><p>Each of the next $n$ lines contains a binary string of length $m$, describing the symbols of the next row of the table.</p><p>It is guaranteed that the sum of $nm$ for all test cases does not exceed $20000$.</p>

## Output

<p>For each test case print the integer $k$ ($0 \leq k \leq 3nm$)&nbsp;— the number of operations.</p><p>In the each of the next $k$ lines print $6$ integers $x_1, y_1, x_2, y_2, x_3, y_3$ ($1 \leq x_1, x_2, x_3 \leq n, 1 \leq y_1, y_2, y_3 \leq m$) describing the next operation. This operation will be made with three cells $(x_1, y_1)$, $(x_2, y_2)$, $(x_3, y_3)$. These three cells should be different. These three cells should belong into some $2 \times 2$ square.</p>





```input1
5
2 2
10
11
3 3
011
101
110
4 4
1111
0110
0110
1111
5 5
01011
11001
00010
11011
10000
2 3
011
101
```




```output1
1
1 1 2 1 2 2
2 
2 1 3 1 3 2
1 2 1 3 2 3
4
1 1 1 2 2 2 
1 3 1 4 2 3
3 2 4 1 4 2
3 3 4 3 4 4
4
1 2 2 1 2 2 
1 4 1 5 2 5 
4 1 4 2 5 1
4 4 4 5 3 4
2
1 3 2 2 2 3
1 2 2 1 2 2
```



## Note

<p>In the first test case, it is possible to make only one operation with cells $(1, 1)$, $(2, 1)$, $(2, 2)$. After that, all symbols will be equal to $0$.</p><p>In the second test case:</p><ul> <li> operation with cells $(2, 1)$, $(3, 1)$, $(3, 2)$. After it the table will be: <pre class="verbatim"><br>011<br>001<br>000<br></pre> </li><li> operation with cells $(1, 2)$, $(1, 3)$, $(2, 3)$. After it the table will be: <pre class="verbatim"><br>000<br>000<br>000<br></pre> </li></ul><p>In the fifth test case:</p><ul> <li> operation with cells $(1, 3)$, $(2, 2)$, $(2, 3)$. After it the table will be: <pre class="verbatim"><br>010<br>110<br></pre> </li><li> operation with cells $(1, 2)$, $(2, 1)$, $(2, 2)$. After it the table will be: <pre class="verbatim"><br>000<br>000<br></pre> </li></ul>
