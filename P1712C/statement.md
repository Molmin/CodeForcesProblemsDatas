## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">An array is sorted if it has no inversions</span></div><div class="epigraph-source">A Young Boy</div></div><p>You are given an array of $n$ <span class="tex-font-style-bf">positive</span> integers $a_1,a_2,\ldots,a_n$. </p><p>In one operation you do the following: </p><ol> <li> Choose <span class="tex-font-style-bf">any</span> integer $x$. </li><li> For all $i$ such that $a_i = x$, do $a_i := 0$ (assign $0$ to $a_i$). </li></ol><p>Find the minimum number of operations required to sort the array in non-decreasing order.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">positive</span> integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print one integer&nbsp;— the minimum number of operations required to sort the array in non-decreasing order.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">positive</span> integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print one integer&nbsp;— the minimum number of operations required to sort the array in non-decreasing order.</p>





```input1|2,3,6,7,10,11
5
3
3 3 2
4
1 3 1 3
5
4 1 5 3 2
4
2 4 1 2
1
1
```




```output1
1
2
4
3
0
```



## Note

<p>In the first test case, you can choose $x = 3$ for the operation, the resulting array is $[0, 0, 2]$.</p><p>In the second test case, you can choose $x = 1$ for the first operation and $x = 3$ for the second operation, the resulting array is $[0, 0, 0, 0]$.</p>
