## Description

<div><p>You are given an array $a_1, a_2, \dots, a_n$, consisting of $n$ integers. You are also given an integer value $x$.</p><p>Let $f(k)$ be the maximum sum of a contiguous subarray of $a$ after applying the following operation: add $x$ to the elements on exactly $k$ <span class="tex-font-style-bf">distinct</span> positions. An empty subarray should also be considered, it has sum $0$.</p><p>Note that the subarray doesn't have to include all of the increased elements.</p><p>Calculate the maximum value of $f(k)$ for all $k$ from $0$ to $n$ independently.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of testcases.</p><p>The first line of the testcase contains two integers $n$ and $x$ ($1 \le n \le 5000$; $0 \le x \le 10^5$)&nbsp;— the number of elements in the array and the value to add.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^5 \le a_i \le 10^5$).</p><p>The sum of $n$ over all testcases doesn't exceed $5000$.</p></div><div class="output-specification"><p>For each testcase, print $n + 1$ integers&nbsp;— the maximum value of $f(k)$ for all $k$ from $0$ to $n$ independently.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of testcases.</p><p>The first line of the testcase contains two integers $n$ and $x$ ($1 \le n \le 5000$; $0 \le x \le 10^5$)&nbsp;— the number of elements in the array and the value to add.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^5 \le a_i \le 10^5$).</p><p>The sum of $n$ over all testcases doesn't exceed $5000$.</p>

## Output

<p>For each testcase, print $n + 1$ integers&nbsp;— the maximum value of $f(k)$ for all $k$ from $0$ to $n$ independently.</p>





```input1
3
4 2
4 1 3 2
3 5
-2 -7 -1
10 2
-6 -1 -2 4 -6 -1 -4 4 -5 -4
```




```output1
10 12 14 16 18
0 4 4 5
4 6 6 7 7 7 7 8 8 8 8
```



## Note

<p>In the first testcase, it doesn't matter which elements you add $x$ to. The subarray with the maximum sum will always be the entire array. If you increase $k$ elements by $x$, $k \cdot x$ will be added to the sum.</p><p>In the second testcase: </p><ul> <li> For $k = 0$, the empty subarray is the best option. </li><li> For $k = 1$, it's optimal to increase the element at position $3$. The best sum becomes $-1 + 5 = 4$ for a subarray $[3, 3]$. </li><li> For $k = 2$, it's optimal to increase the element at position $3$ and any other element. The best sum is still $4$ for a subarray $[3, 3]$. </li><li> For $k = 3$, you have to increase all elements. The best sum becomes $(-2 + 5) + (-7 + 5) + (-1 + 5) = 5$ for a subarray $[1, 3]$. </li></ul>
