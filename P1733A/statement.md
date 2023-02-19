## Description

<div><p>You are given an array $a$ with $n$ integers. You can perform the following operation at most $k$ times:</p><ul> <li> Choose two indices $i$ and $j$, in which $i \,\bmod\, k = j \,\bmod\, k$ ($1 \le i &lt; j \le n$). </li><li> Swap $a_i$ and $a_j$. </li></ul><p>After performing all operations, you have to select $k$ consecutive elements, and the sum of the $k$ elements becomes your score. Find the maximum score you can get.</p><p>Here $x \bmod y$ denotes the remainder from dividing $x$ by $y$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 600$)&nbsp;— the number of test cases.</p><p>Each test case consists of two lines. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 100$)&nbsp;— the length of the array and the number in the statement above.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) &nbsp;— the array itself.</p></div><div class="output-specification"><p>For each test case, print the maximum score you can get, one per line.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 600$)&nbsp;— the number of test cases.</p><p>Each test case consists of two lines. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 100$)&nbsp;— the length of the array and the number in the statement above.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) &nbsp;— the array itself.</p>

## Output

<p>For each test case, print the maximum score you can get, one per line.</p>





```input1|2,3,6,7,10,11
5
3 2
5 6 0
1 1
7
5 3
7 0 4 0 4
4 2
2 7 3 4
3 3
1000000000 1000000000 999999997
```




```output1
11
7
15
10
2999999997
```



## Note

<p>In the first test case, we can get a score of $11$ if we select $a_1, a_2$ without performing any operations.</p><p>In the third test case, we can get a score of $15$ if we first swap $a_1$ with $a_4$ and then select $a_3, a_4, a_5$. </p>
