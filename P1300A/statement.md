## Description

<div><p>Guy-Manuel and Thomas have an array $a$ of $n$ integers [$a_1, a_2, \dots, a_n$]. In one step they can add $1$ to any element of the array. Formally, in one step they can choose any integer index $i$ ($1 \le i \le n$) and do $a_i := a_i + 1$.</p><p><span class="tex-font-style-it">If either the sum or the product of all elements in the array is equal to zero, Guy-Manuel and Thomas do not mind to do this operation one more time.</span></p><p>What is the minimum number of steps they need to do to make both the sum and the product of all elements in the array <span class="tex-font-style-bf">different from zero</span>? Formally, find the minimum number of steps to make $a_1 + a_2 +$ $\dots$ $+ a_n \ne 0$ and $a_1 \cdot a_2 \cdot$ $\dots$ $\cdot a_n \ne 0$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$)&nbsp;— the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-100 \le a_i \le 100$)&nbsp;— elements of the array .</p></div><div class="output-specification"><p>For each test case, output the minimum number of steps required to make both sum and product of all elements in the array different from zero.</p></div>

## Input

<p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$)&nbsp;— the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-100 \le a_i \le 100$)&nbsp;— elements of the array .</p>

## Output

<p>For each test case, output the minimum number of steps required to make both sum and product of all elements in the array different from zero.</p>





```input1
4
3
2 -1 -1
4
-1 0 0 1
2
-1 2
3
0 -2 1
```




```output1
1
2
0
2
```



## Note

<p>In the first test case, the sum is $0$. If we add $1$ to the first element, the array will be $[3,-1,-1]$, the sum will be equal to $1$ and the product will be equal to $3$.</p><p>In the second test case, both product and sum are $0$. If we add $1$ to the second and the third element, the array will be $[-1,1,1,1]$, the sum will be equal to $2$ and the product will be equal to $-1$. It can be shown that fewer steps can't be enough.</p><p>In the third test case, both sum and product are non-zero, we don't need to do anything.</p><p>In the fourth test case, after adding $1$ twice to the first element the array will be $[2,-2,1]$, the sum will be $1$ and the product will be $-4$.</p>
