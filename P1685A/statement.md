## Description

<div><p>You are given $n$ integers $a_1, a_2, \ldots, a_n$. Is it possible to arrange them on a circle so that each number is strictly greater than both its neighbors or strictly smaller than both its neighbors?</p><p>In other words, check if there exists a rearrangement $b_1, b_2, \ldots, b_n$ of the integers $a_1, a_2, \ldots, a_n$ such that for each $i$ from $1$ to $n$ at least one of the following conditions holds:</p><ul><li> $b_{i-1} &lt; b_i &gt; b_{i+1}$</li><li> $b_{i-1} &gt; b_i &lt; b_{i+1}$</li></ul><p>To make sense of the previous formulas for $i=1$ and $i=n$, one shall define $b_0=b_n$ and $b_{n+1}=b_1$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 3\cdot 10^4$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 10^5$) &nbsp;— the number of integers.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$).</p><p>The sum of $n$ over all test cases doesn't exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if it is not possible to arrange the numbers on the circle satisfying the conditions from the statement, output $\texttt{NO}$. You can output each letter in any case.</p><p>Otherwise, output $\texttt{YES}$. In the second line, output $n$ integers $b_1, b_2, \ldots, b_n$, which are a rearrangement of $a_1, a_2, \ldots, a_n$ and satisfy the conditions from the statement. If there are multiple valid ways to arrange the numbers, you can output any of them.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 3\cdot 10^4$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 10^5$) &nbsp;— the number of integers.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$).</p><p>The sum of $n$ over all test cases doesn't exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, if it is not possible to arrange the numbers on the circle satisfying the conditions from the statement, output $\texttt{NO}$. You can output each letter in any case.</p><p>Otherwise, output $\texttt{YES}$. In the second line, output $n$ integers $b_1, b_2, \ldots, b_n$, which are a rearrangement of $a_1, a_2, \ldots, a_n$ and satisfy the conditions from the statement. If there are multiple valid ways to arrange the numbers, you can output any of them.</p>





```input1
4
3
1 1 2
4
1 9 8 4
4
2 0 2 2
6
1 1 1 11 111 1111
```




```output1
NO
YES
1 8 4 9 
NO
YES
1 11 1 111 1 1111
```



## Note

<p>It can be shown that there are no valid arrangements for the first and the third test cases.</p><p>In the second test case, the arrangement $[1, 8, 4, 9]$ works. In this arrangement, $1$ and $4$ are both smaller than their neighbors, and $8, 9$ are larger.</p><p>In the fourth test case, the arrangement $[1, 11, 1, 111, 1, 1111]$ works. In this arrangement, the three elements equal to $1$ are smaller than their neighbors, while all other elements are larger than their neighbors.</p>
