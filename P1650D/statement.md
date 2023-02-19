## Description

<div><p>Petya got an array $a$ of numbers from $1$ to $n$, where $a[i]=i$.</p><p>He performed $n$ operations sequentially. In the end, he received a new state of the $a$ array.</p><p>At the $i$-th operation, Petya chose the first $i$ elements of the array and cyclically shifted them to the right an arbitrary number of times (elements with indexes $i+1$ and more remain in their places). One cyclic shift to the right is such a transformation that the array $a=[a_1, a_2, \dots, a_n]$ becomes equal to the array $a = [a_i, a_1, a_2, \dots, a_{i-2}, a_{i-1}, a_{i+1}, a_{i+2}, \dots, a_n]$.</p><p>For example, if $a = [5,4,2,1,3]$ and $i=3$ (that is, this is the third operation), then as a result of this operation, he could get any of these three arrays:</p><ul> <li> $a = [5,4,2,1,3]$ (makes $0$ cyclic shifts, or any number that is divisible by $3$); </li><li> $a = [2,5,4,1,3]$ (makes $1$ cyclic shift, or any number that has a remainder of $1$ when divided by $3$); </li><li> $a = [4,2,5,1,3]$ (makes $2$ cyclic shifts, or any number that has a remainder of $2$ when divided by $3$). </li></ul><p>Let's look at an example. Let $n=6$, i.e. initially $a=[1,2,3,4,5,6]$. A possible scenario is described below.</p><ul> <li> $i=1$: no matter how many cyclic shifts Petya makes, the array $a$ does not change. </li><li> $i=2$: let's say Petya decided to make a $1$ cyclic shift, then the array will look like $a = [\textbf{2}, \textbf{1}, 3, 4, 5, 6]$. </li><li> $i=3$: let's say Petya decided to make $1$ cyclic shift, then the array will look like $a = [\textbf{3}, \textbf{2}, \textbf{1}, 4, 5, 6]$. </li><li> $i=4$: let's say Petya decided to make $2$ cyclic shifts, the original array will look like $a = [\textbf{1}, \textbf{4}, \textbf{3}, \textbf{2}, 5, 6]$. </li><li> $i=5$: let's say Petya decided to make $0$ cyclic shifts, then the array won't change. </li><li> $i=6$: let's say Petya decided to make $4$ cyclic shifts, the array will look like $a = [\textbf{3}, \textbf{2}, \textbf{5}, \textbf{6}, \textbf{1}, \textbf{4}]$. </li></ul><p>You are given a final array state $a$ after all $n$ operations. Determine if there is a way to perform the operation that produces this result. In this case, if an answer exists, print the numbers of cyclical shifts that occurred during each of the $n$ operations.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of the description of each test case contains one integer $n$ ($2 \le n \le 2\cdot10^3$)&nbsp;— the length of the array $a$.</p><p>The next line contains the final state of the array $a$: $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) are written. All $a_i$ are distinct.</p><p>It is guaranteed that the sum of $n$ values over all test cases does not exceed $2\cdot10^3$.</p></div><div class="output-specification"><p>For each test case, print the answer on a separate line.</p><p>Print <span class="tex-font-style-tt">-1</span> if the given final value $a$ cannot be obtained by performing an arbitrary number of cyclic shifts on each operation. Otherwise, print $n$ non-negative integers $d_1, d_2, \dots, d_n$ ($d_i \ge 0$), where $d_i$ means that during the $i$-th operation the first $i$ elements of the array were cyclic shifted to the right $d_i$ times.</p><p>If there are several possible answers, print the one where the total number of shifts is minimal (that is, the sum of $d_i$ values is the smallest). If there are several such answers, print any of them.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of the description of each test case contains one integer $n$ ($2 \le n \le 2\cdot10^3$)&nbsp;— the length of the array $a$.</p><p>The next line contains the final state of the array $a$: $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) are written. All $a_i$ are distinct.</p><p>It is guaranteed that the sum of $n$ values over all test cases does not exceed $2\cdot10^3$.</p>

## Output

<p>For each test case, print the answer on a separate line.</p><p>Print <span class="tex-font-style-tt">-1</span> if the given final value $a$ cannot be obtained by performing an arbitrary number of cyclic shifts on each operation. Otherwise, print $n$ non-negative integers $d_1, d_2, \dots, d_n$ ($d_i \ge 0$), where $d_i$ means that during the $i$-th operation the first $i$ elements of the array were cyclic shifted to the right $d_i$ times.</p><p>If there are several possible answers, print the one where the total number of shifts is minimal (that is, the sum of $d_i$ values is the smallest). If there are several such answers, print any of them.</p>





```input1
3
6
3 2 5 6 1 4
3
3 1 2
8
5 8 1 3 2 6 4 7
```




```output1
0 1 1 2 0 4 
0 0 1 
0 1 2 0 2 5 6 2
```



## Note

<p>The first test case matches the example from the statement.</p><p>The second set of input data is simple. Note that the answer $[3, 2, 1]$ also gives the same permutation, but since the total number of shifts $3+2+1$ is greater than $0+0+1$, this answer is not correct.</p>
