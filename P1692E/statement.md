## Description

<div><p>Slavic has an array of length $n$ consisting only of zeroes and ones. In one operation, he removes either the first or the last element of the array. </p><p>What is the minimum number of operations Slavic has to perform such that the total sum of the array is equal to $s$ after performing all the operations? In case the sum $s$ can't be obtained after any amount of operations, you should output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $s$ ($1 \leq n, s \leq 2 \cdot 10^5$)&nbsp;— the length of the array and the needed sum of elements.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 1$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the minimum amount of operations required to have the total sum of the array equal to $s$, or <span class="tex-font-style-tt">-1</span> if obtaining an array with sum $s$ isn't possible.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $s$ ($1 \leq n, s \leq 2 \cdot 10^5$)&nbsp;— the length of the array and the needed sum of elements.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 1$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the minimum amount of operations required to have the total sum of the array equal to $s$, or <span class="tex-font-style-tt">-1</span> if obtaining an array with sum $s$ isn't possible.</p>





```input1
7
3 1
1 0 0
3 1
1 1 0
9 3
0 1 0 1 1 1 0 0 1
6 4
1 1 1 1 1 1
5 1
0 0 1 1 0
16 2
1 1 0 0 1 0 0 1 1 0 0 0 0 0 1 1
6 3
1 0 1 0 0 0
```




```output1
0
1
3
2
2
7
-1
```



## Note

<p>In the first test case, the sum of the whole array is $1$ from the beginning, so we don't have to make any operations.</p><p>In the second test case, the sum of the array is $2$ and we want it to be equal to $1$, so we should remove the first element. The array turns into $[1, 0]$, which has a sum equal to $1$.</p><p>In the third test case, the sum of the array is $5$ and we need it to be $3$. We can obtain such a sum by removing the first two elements and the last element, doing a total of three operations. The array turns into $[0, 1, 1, 1, 0, 0]$, which has a sum equal to $3$.</p>
