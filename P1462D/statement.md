## Description

<div><p>Polycarp was given an array of $a[1 \dots n]$ of $n$ integers. He can perform the following operation with the array $a$ no more than $n$ times:</p><ul> <li> Polycarp selects the index $i$ and adds the value $a_i$ to <span class="tex-font-style-bf">one of his choice</span> of its neighbors. More formally, Polycarp adds the value of $a_i$ to $a_{i-1}$ or to $a_{i+1}$ (if such a neighbor does not exist, then it is impossible to add to it). </li><li> After adding it, Polycarp removes the $i$-th element from the $a$ array. During this step the length of $a$ is decreased by $1$. </li></ul><p>The two items above together denote one single operation.</p><p>For example, if Polycarp has an array $a = [3, 1, 6, 6, 2]$, then it can perform the following sequence of operations with it: </p><ul> <li> Polycarp selects $i = 2$ and adds the value $a_i$ to $(i-1)$-th element: $a = [4, 6, 6, 2]$. </li><li> Polycarp selects $i = 1$ and adds the value $a_i$ to $(i+1)$-th element: $a = [10, 6, 2]$. </li><li> Polycarp selects $i = 3$ and adds the value $a_i$ to $(i-1)$-th element: $a = [10, 8]$. </li><li> Polycarp selects $i = 2$ and adds the value $a_i$ to $(i-1)$-th element: $a = [18]$. </li></ul><p>Note that Polycarp could stop performing operations at any time.</p><p>Polycarp wondered how many minimum operations he would need to perform to make all the elements of $a$ equal (i.e., he wants all $a_i$ are equal to each other).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 3000$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 3000$)&nbsp;— the length of the array. The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^5$)&nbsp;— array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3000$.</p></div><div class="output-specification"><p>For each test case, output a single number&nbsp;— the minimum number of operations that Polycarp needs to perform so that all elements of the $a$ array are the same (equal).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 3000$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 3000$)&nbsp;— the length of the array. The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^5$)&nbsp;— array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3000$.</p>

## Output

<p>For each test case, output a single number&nbsp;— the minimum number of operations that Polycarp needs to perform so that all elements of the $a$ array are the same (equal).</p>





```input1
4
5
3 1 6 6 2
4
1 2 2 1
3
2 2 2
4
6 3 2 1
```




```output1
4
2
0
2
```



## Note

<p>In the first test case of the example, the answer can be constructed like this (just one way among many other ways):</p><p>$[3, 1, 6, 6, 2]$ $\xrightarrow[]{i=4,~add~to~left}$ $[3, 1, 12, 2]$ $\xrightarrow[]{i=2,~add~to~right}$ $[3, 13, 2]$ $\xrightarrow[]{i=1,~add~to~right}$ $[16, 2]$ $\xrightarrow[]{i=2,~add~to~left}$ $[18]$. All elements of the array $[18]$ are the same.</p><p>In the second test case of the example, the answer can be constructed like this (just one way among other ways):</p><p>$[1, 2, 2, 1]$ $\xrightarrow[]{i=1,~add~to~right}$ $[3, 2, 1]$ $\xrightarrow[]{i=3,~add~to~left}$ $[3, 3]$. All elements of the array $[3, 3]$ are the same.</p><p>In the third test case of the example, Polycarp doesn't need to perform any operations since $[2, 2, 2]$ contains equal (same) elements only.</p><p>In the fourth test case of the example, the answer can be constructed like this (just one way among other ways):</p><p>$[6, 3, 2, 1]$ $\xrightarrow[]{i=3,~add~to~right}$ $[6, 3, 3]$ $\xrightarrow[]{i=3,~add~to~left}$ $[6, 6]$. All elements of the array $[6, 6]$ are the same.</p>
