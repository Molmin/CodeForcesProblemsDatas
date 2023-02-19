## Description

<div><p>Dmitry has an array of $n$ non-negative integers $a_1, a_2, \dots, a_n$.</p><p>In one operation, Dmitry can choose any index $j$ ($1 \le j \le n$) and increase the value of the element $a_j$ by $1$. He can choose the same index $j$ multiple times.</p><p>For each $i$ from $0$ to $n$, determine whether Dmitry can make the $\mathrm{MEX}$ of the array equal to exactly $i$. If it is possible, then determine the minimum number of operations to do it.</p><p>The $\mathrm{MEX}$ of the array is equal to the minimum non-negative integer that is not in the array. For example, the $\mathrm{MEX}$ of the array $[3, 1, 0]$ is equal to $2$, and the array $[3, 3, 1, 4]$ is equal to $0$.</p></div><div class="input-specification"><p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the input. </p><p>The descriptions of the test cases follow.</p><p>The first line of the description of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of the description of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le n$)&nbsp;— elements of the array $a$.</p><p>It is guaranteed that the sum of the values $n$ over all test cases in the test does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, output $n + 1$ integer&nbsp;— $i$-th number is equal to the minimum number of operations for which you can make the array $\mathrm{MEX}$ equal to $i$ ($0 \le i \le n$), or <span class="tex-font-style-tt">-1</span> if this cannot be done.</p></div>

## Input

<p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the input. </p><p>The descriptions of the test cases follow.</p><p>The first line of the description of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line of the description of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le n$)&nbsp;— elements of the array $a$.</p><p>It is guaranteed that the sum of the values $n$ over all test cases in the test does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, output $n + 1$ integer&nbsp;— $i$-th number is equal to the minimum number of operations for which you can make the array $\mathrm{MEX}$ equal to $i$ ($0 \le i \le n$), or <span class="tex-font-style-tt">-1</span> if this cannot be done.</p>





```input1
5
3
0 1 3
7
0 1 2 3 4 3 2
4
3 0 0 0
7
4 6 2 3 5 0 5
5
4 0 1 0 4
```




```output1
1 1 0 -1 
1 1 2 2 1 0 2 6 
3 0 1 4 3 
1 0 -1 -1 -1 -1 -1 -1 
2 1 0 2 -1 -1
```



## Note

<p>In the first set of example inputs, $n=3$:</p><ul> <li> to get $\mathrm{MEX}=0$, it is enough to perform one increment: $a_1$<span class="tex-font-style-tt">++</span>; </li><li> to get $\mathrm{MEX}=1$, it is enough to perform one increment: $a_2$<span class="tex-font-style-tt">++</span>; </li><li> $\mathrm{MEX}=2$ for a given array, so there is no need to perform increments; </li><li> it is impossible to get $\mathrm{MEX}=3$ by performing increments. </li></ul>
