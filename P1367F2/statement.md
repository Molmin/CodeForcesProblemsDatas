## Description

<div><p><span class="tex-font-style-bf">This is a hard version of the problem. In this version, the given array can contain equal elements and the constraints on $n$ are greater than in the easy version of the problem.</span></p><p>You are given an array $a$ of $n$ integers <span class="tex-font-style-bf">(the given array can contain equal elements)</span>. You can perform the following operations on array elements:</p><ol> <li> choose any index $i$ ($1 \le i \le n$) and move the element $a[i]$ to the <span class="tex-font-style-bf">begin</span> of the array; </li><li> choose any index $i$ ($1 \le i \le n$) and move the element $a[i]$ to the <span class="tex-font-style-bf">end</span> of the array. </li></ol><p>For example, if $n = 5$, $a = [4, 7, 2, 2, 9]$, then the following sequence of operations can be performed: </p><ul> <li> after performing the operation of the first type to the second element, the array $a$ will become $[7, 4, 2, 2, 9]$; </li><li> after performing the operation of the second type to the second element, the array $a$ will become $[7, 2, 2, 9, 4]$. </li></ul><p>You can perform operations of any type any number of times in any order.</p><p>Find the minimum total number of operations of the first and second type that will make the $a$ array sorted in non-decreasing order. In other words, what is the minimum number of operations must be performed so the array satisfies the inequalities $a[1] \le a[2] \le \ldots \le a[n]$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>Each test case starts with a line containing an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of the array $a$.</p><p>Then follow $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— an array that needs to be sorted by the given operations. <span class="tex-font-style-bf">The given array can contain equal elements</span>.</p><p>The sum of $n$ for all test cases in one test does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output one integer&nbsp;— the minimum total number of operations of the first and second type, which will make the array sorted in non-decreasing order.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>Each test case starts with a line containing an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of the array $a$.</p><p>Then follow $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— an array that needs to be sorted by the given operations. <span class="tex-font-style-bf">The given array can contain equal elements</span>.</p><p>The sum of $n$ for all test cases in one test does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output one integer&nbsp;— the minimum total number of operations of the first and second type, which will make the array sorted in non-decreasing order.</p>





```input1
9
5
4 7 2 2 9
5
3 5 8 1 7
5
1 2 2 4 5
2
0 1
3
0 1 0
4
0 1 0 0
4
0 1 0 1
4
0 1 0 2
20
16 15 1 10 0 14 0 10 3 9 2 5 4 5 17 9 10 20 0 9
```




```output1
2
2
0
0
1
1
1
1
16
```



## Note

<p>In the first test case, you first need to move two <span class="tex-font-style-tt">2</span>, to the beginning of the array. Therefore, the desired sequence of operations: $[4, 7, 2, 2, 9] \rightarrow [2, 4, 7, 2, 9] \rightarrow [2, 2, 4, 7, 9]$.</p><p>In the second test case, you need to move the <span class="tex-font-style-tt">1</span> to the beginning of the array, and the <span class="tex-font-style-tt">8</span>&nbsp;— to the end. Therefore, the desired sequence of operations: $[3, 5, 8, 1, 7] \rightarrow [1, 3, 5, 8, 7] \rightarrow [1, 3, 5, 7, 8]$.</p><p>In the third test case, the array is already sorted.</p>
