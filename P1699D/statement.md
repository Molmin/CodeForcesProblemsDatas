## Description

<div><p>You are given an integer $n$ and an array $a_1,a_2,\ldots,a_n$.</p><p>In one operation, you can choose an index $i$ ($1 \le i \lt n$) for which $a_i \neq a_{i+1}$ and delete both $a_i$ and $a_{i+1}$ from the array. After deleting $a_i$ and $a_{i+1}$, the remaining parts of the array are concatenated.</p><p>For example, if $a=[1,4,3,3,6,2]$, then after performing an operation with $i=2$, the resulting array will be $[1,3,6,2]$.</p><p>What is the maximum possible length of an array of <span class="tex-font-style-bf">equal</span> elements obtainable from $a$ by performing several (perhaps none) of the aforementioned operations?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The following lines contain the descriptions of the test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of array $a$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10\,000$.</p></div><div class="output-specification"><p>For each testcase, print a single integer, the maximum possible length of an array of <span class="tex-font-style-bf">equal</span> elements obtainable from $a$ by performing a sequence of operations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The following lines contain the descriptions of the test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of array $a$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10\,000$.</p>

## Output

<p>For each testcase, print a single integer, the maximum possible length of an array of <span class="tex-font-style-bf">equal</span> elements obtainable from $a$ by performing a sequence of operations.</p>





```input1|2,3,6,7,10,11
5
7
1 2 3 2 1 3 3
1
1
6
1 1 1 2 2 2
8
1 1 2 2 3 3 1 1
12
1 5 2 3 3 3 4 4 4 4 3 3
```




```output1
3
1
0
4
2
```



## Note

<p>For the first testcase, an optimal sequence of operations would be: $[1,2,3,2,1,3,3] \rightarrow [3,2,1,3,3] \rightarrow [3,3,3]$.</p><p>For the second testcase, all elements in the array are already equal.</p><p>For the third testcase, the only possible sequence of operations is: $[1,1,1,2,2,2] \rightarrow [1,1,2,2] \rightarrow [1,2] \rightarrow []$. Note that, according to the statement, the elements deleted at each step must be different.</p><p>For the fourth testcase, the optimal sequence of operations is: $[1,1,2,2,3,3,1,1] \rightarrow [1,1,2,3,1,1] \rightarrow [1,1,1,1]$.</p><p>For the fifth testcase, one possible reachable array of two equal elements is $[4,4]$.</p>
