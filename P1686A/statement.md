## Description

<div><p>You are given an array of $n$ integers $a_1, a_2, \ldots, a_n$. After you watched the amazing film "Everything Everywhere All At Once", you came up with the following operation.</p><p>In one operation, you choose $n-1$ elements of the array and replace each of them with their arithmetic mean (which doesn't have to be an integer). For example, from the array $[1, 2, 3, 1]$ we can get the array $[2, 2, 2, 1]$, if we choose the first three elements, or we can get the array $[\frac{4}{3}, \frac{4}{3}, 3, \frac{4}{3}]$, if we choose all elements except the third.</p><p>Is it possible to make all elements of the array equal by performing a finite number of such operations?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 200$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 50$) &nbsp;— the number of integers.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 100$).</p></div><div class="output-specification"><p>For each test case, if it is possible to make all elements equal after some number of operations, output $\texttt{YES}$. Otherwise, output $\texttt{NO}$.</p><p>You can output $\texttt{YES}$ and $\texttt{NO}$ in any case (for example, strings $\texttt{yEs}$, $\texttt{yes}$, $\texttt{Yes}$ will be recognized as a positive response).</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 200$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 50$) &nbsp;— the number of integers.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 100$).</p>

## Output

<p>For each test case, if it is possible to make all elements equal after some number of operations, output $\texttt{YES}$. Otherwise, output $\texttt{NO}$.</p><p>You can output $\texttt{YES}$ and $\texttt{NO}$ in any case (for example, strings $\texttt{yEs}$, $\texttt{yes}$, $\texttt{Yes}$ will be recognized as a positive response).</p>





```input1|2,3,6,7
4
3
42 42 42
5
1 2 3 4 5
4
4 3 2 1
3
24 2 22
```




```output1
YES
YES
NO
NO
```



## Note

<p>In the first test case, all elements are already equal.</p><p>In the second test case, you can choose all elements except the third, their average is $\frac{1 + 2 + 4 + 5}{4} = 3$, so the array will become $[3, 3, 3, 3, 3]$.</p><p>It's possible to show that it's impossible to make all elements equal in the third and fourth test cases.</p>
