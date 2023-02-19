## Description

<div><p>An array is <span class="tex-font-style-it">beautiful</span> if both of the following two conditions meet:</p><ul> <li> there are <span class="tex-font-style-bf">at least</span> $l_1$ and <span class="tex-font-style-bf">at most</span> $r_1$ elements in the array equal to its minimum; </li><li> there are <span class="tex-font-style-bf">at least</span> $l_2$ and <span class="tex-font-style-bf">at most</span> $r_2$ elements in the array equal to its maximum. </li></ul><p>For example, the array $[2, 3, 2, 4, 4, 3, 2]$ has $3$ elements equal to its minimum ($1$-st, $3$-rd and $7$-th) and $2$ elements equal to its maximum ($4$-th and $5$-th).</p><p>Another example: the array $[42, 42, 42]$ has $3$ elements equal to its minimum and $3$ elements equal to its maximum.</p><p>Your task is to calculate the <span class="tex-font-style-bf">minimum</span> possible number of elements in a <span class="tex-font-style-it">beautiful</span> array.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line containing four integers $l_1$, $r_1$, $l_2$ and $r_2$ ($1 \le l_1 \le r_1 \le 50$; $1 \le l_2 \le r_2 \le 50$).</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the minimum possible number of elements in a beautiful array.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line containing four integers $l_1$, $r_1$, $l_2$ and $r_2$ ($1 \le l_1 \le r_1 \le 50$; $1 \le l_2 \le r_2 \le 50$).</p>

## Output

<p>For each test case, print one integer&nbsp;— the minimum possible number of elements in a beautiful array.</p>





```input1
7
3 5 4 6
5 8 5 5
3 3 10 12
1 5 3 3
1 1 2 2
2 2 1 1
6 6 6 6
```




```output1
4
5
13
3
3
3
6
```



## Note

<p>Optimal arrays in the test cases of the example:</p><ol> <li> $[1, 1, 1, 1]$, it has $4$ minimums and $4$ maximums; </li><li> $[4, 4, 4, 4, 4]$, it has $5$ minimums and $5$ maximums; </li><li> $[1, 2, 1, 2, 2, 1, 2, 2, 2, 2, 2, 2, 2]$, it has $3$ minimums and $10$ maximums; </li><li> $[8, 8, 8]$, it has $3$ minimums and $3$ maximums; </li><li> $[4, 6, 6]$, it has $1$ minimum and $2$ maximums; </li><li> $[3, 4, 3]$, it has $2$ minimums and $1$ maximum; </li><li> $[5, 5, 5, 5, 5, 5]$, it has $6$ minimums and $6$ maximums. </li></ol>
