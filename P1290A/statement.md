## Description

<div><p>You and your $n - 1$ friends have found an array of integers $a_1, a_2, \dots, a_n$. You have decided to share it in the following way: All $n$ of you stand in a line in a particular order. Each minute, the person at the front of the line chooses either the first or the last element of the array, removes it, and keeps it for himself. He then gets out of line, and the next person in line continues the process.</p><p>You are standing in the $m$-th position in the line. <span class="tex-font-style-bf">Before the process starts</span>, you may choose up to $k$ different people in the line, and persuade them to always take either the first or the last element in the array on their turn (for each person his own choice, not necessarily equal for all people), no matter what the elements themselves are. <span class="tex-font-style-bf">Once the process starts, you cannot persuade any more people, and you cannot change the choices for the people you already persuaded</span>.</p><p>Suppose that you're doing your choices optimally. What is the greatest integer $x$ such that, no matter what are the choices of the friends you didn't choose to control, the element you will take from the array will be <span class="tex-font-style-underline">greater than or equal to</span> $x$?</p><p>Please note that the friends you don't control may do their choice <span class="tex-font-style-bf"><span class="tex-font-style-underline">arbitrarily</span></span>, and they will not necessarily take the biggest element available.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains three space-separated integers $n$, $m$ and $k$ ($1 \le m \le n \le 3500$, $0 \le k \le n - 1$) &nbsp;— the number of elements in the array, your position in line and the number of people whose choices you can fix.</p><p>The second line of each test case contains $n$ positive integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) &nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3500$.</p></div><div class="output-specification"><p>For each test case, print the largest integer $x$ such that you can guarantee to obtain at least $x$.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains three space-separated integers $n$, $m$ and $k$ ($1 \le m \le n \le 3500$, $0 \le k \le n - 1$) &nbsp;— the number of elements in the array, your position in line and the number of people whose choices you can fix.</p><p>The second line of each test case contains $n$ positive integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) &nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3500$.</p>

## Output

<p>For each test case, print the largest integer $x$ such that you can guarantee to obtain at least $x$.</p>





```input1
4
6 4 2
2 9 2 3 8 5
4 4 1
2 13 60 4
4 1 3
1 2 2 1
2 2 0
1 2
```




```output1
8
4
1
1
```



## Note

<p>In the first test case, an optimal strategy is to force the first person to take the last element and the second person to take the first element.</p><ul> <li> the first person will take the last element ($5$) because he or she was forced by you to take the last element. After this turn the remaining array will be $[2, 9, 2, 3, 8]$; </li><li> the second person will take the first element ($2$) because he or she was forced by you to take the first element. After this turn the remaining array will be $[9, 2, 3, 8]$; </li><li> if the third person will choose to take the first element ($9$), at your turn the remaining array will be $[2, 3, 8]$ and you will take $8$ (the last element); </li><li> if the third person will choose to take the last element ($8$), at your turn the remaining array will be $[9, 2, 3]$ and you will take $9$ (the first element). </li></ul><p>Thus, this strategy guarantees to end up with at least $8$. We can prove that there is no strategy that guarantees to end up with at least $9$. Hence, the answer is $8$.</p><p>In the second test case, an optimal strategy is to force the first person to take the first element. Then, in the worst case, both the second and the third person will take the first element: you will end up with $4$.</p>
