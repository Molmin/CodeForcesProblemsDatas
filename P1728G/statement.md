## Description

<div><p>Consider a segment $[0, d]$ of the coordinate line. There are $n$ lanterns and $m$ points of interest in this segment.</p><p>For each lantern, you can choose its power — an integer between $0$ and $d$ (inclusive). A lantern with coordinate $x$ illuminates the point of interest with coordinate $y$ if $|x - y|$ is less than or equal to the power of the lantern.</p><p>A way to choose the power values for all lanterns is considered <span class="tex-font-style-bf">valid</span> if every point of interest is illuminated by at least one lantern.</p><p>You have to process $q$ queries. Each query is represented by one integer $f_i$. To answer the $i$-th query, you have to:</p><ul> <li> add a lantern on coordinate $f_i$; </li><li> calculate the number of valid ways to assign power values to all lanterns, and print it modulo $998244353$; </li><li> remove the lantern you just added. </li></ul></div><div class="input-specification"><p>The first line contains three integers $d$, $n$ and $m$ ($4 \le d \le 3 \cdot 10^5$; $1 \le n \le 2 \cdot 10^5$; $1 \le m \le 16$) — the size of the segment, the number of lanterns and the number of points of interest, respectively.</p><p>The second line contains $n$ integers $l_1, l_2, \dots, l_n$ ($1 \le l_i \le d - 1$), where $l_i$ is the coordinate of the $i$-th lantern.</p><p>The third line contains $m$ integers $p_1, p_2, \dots, p_m$ ($1 \le p_i \le d - 1$), where $p_i$ is the coordinate of the $i$-th point of interest.</p><p>The fourth line contains one integer $q$ ($1 \le q \le 5 \cdot 10^5$) — the number of queries.</p><p>The fifth line contains $q$ integers $f_1, f_2, \dots, f_q$ ($1 \le f_i \le d - 1$), where $f_i$ is the integer representing the $i$-th query.</p><p>Additional constraint on the input: during the processing of each query, no coordinate contains more than one object (i. e. there cannot be two or more lanterns with the same coordinate, two or more points of interest with the same coordinate, or a lantern and a point of interest with the same coordinate).</p></div><div class="output-specification"><p>For each query, print one integer — the answer to it, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains three integers $d$, $n$ and $m$ ($4 \le d \le 3 \cdot 10^5$; $1 \le n \le 2 \cdot 10^5$; $1 \le m \le 16$) — the size of the segment, the number of lanterns and the number of points of interest, respectively.</p><p>The second line contains $n$ integers $l_1, l_2, \dots, l_n$ ($1 \le l_i \le d - 1$), where $l_i$ is the coordinate of the $i$-th lantern.</p><p>The third line contains $m$ integers $p_1, p_2, \dots, p_m$ ($1 \le p_i \le d - 1$), where $p_i$ is the coordinate of the $i$-th point of interest.</p><p>The fourth line contains one integer $q$ ($1 \le q \le 5 \cdot 10^5$) — the number of queries.</p><p>The fifth line contains $q$ integers $f_1, f_2, \dots, f_q$ ($1 \le f_i \le d - 1$), where $f_i$ is the integer representing the $i$-th query.</p><p>Additional constraint on the input: during the processing of each query, no coordinate contains more than one object (i. e. there cannot be two or more lanterns with the same coordinate, two or more points of interest with the same coordinate, or a lantern and a point of interest with the same coordinate).</p>

## Output

<p>For each query, print one integer — the answer to it, taken modulo $998244353$.</p>





```input1
6 1 1
4
3
3
2 1 5
```




```input2
6 1 2
4
2 5
2
1 3
```




```input3
20 1 2
11
15 7
1
8
```




```input4
20 3 5
5 7 18
1 6 3 10 19
5
4 17 15 8 9
```




```output1
48
47
47
```




```output2
44
46
```




```output3
413
```




```output4
190431
187503
188085
189903
189708
```


