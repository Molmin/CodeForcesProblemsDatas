## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference is that in this version $0 \leq k \leq 20$.</span></p><p>There is an array $a_1, a_2, \ldots, a_n$ of $n$ positive integers. You should divide it into a minimal number of continuous segments, such that in each segment there are no two numbers (on different positions), whose product is a perfect square.</p><p>Moreover, it is allowed to do at most $k$ such operations before the division: choose a number in the array and change its value to any positive integer.</p><p>What is the minimum number of continuous segments you should use if you will make changes optimally?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \le t \le 1000)$ &nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \leq k \leq 20$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^7$).</p><p>It's guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print a single integer &nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \le t \le 1000)$ &nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \leq k \leq 20$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^7$).</p><p>It's guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print a single integer &nbsp;— the answer to the problem.</p>





```input1|2,3,6,7
3
5 2
18 6 2 4 1
11 4
6 2 2 8 9 1 3 6 3 9 7
1 0
1
```




```output1
1
2
1
```



## Note

<p>In the first test case it is possible to change the array this way: $[\underline{3}, 6, 2, 4, \underline{5}]$ (changed elements are underlined). After that the array does not need to be divided, so the answer is $1$.</p><p>In the second test case it is possible to change the array this way: $[6, 2, \underline{3}, 8, 9, \underline{5}, 3, 6, \underline{10}, \underline{11}, 7]$. After that such division is optimal: </p><ul> <li> $[6, 2, 3]$ </li><li> $[8, 9, 5, 3, 6, 10, 11, 7]$ </li></ul>
