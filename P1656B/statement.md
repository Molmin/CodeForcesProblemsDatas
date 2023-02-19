## Description

<div><p>You are given a list of $n$ integers. You can perform the following operation: you choose an element $x$ from the list, erase $x$ from the list, and subtract the value of $x$ from all the remaining elements. Thus, in one operation, the length of the list is decreased by exactly $1$.</p><p>Given an integer $k$ ($k&gt;0$), find if there is some sequence of $n-1$ operations such that, after applying the operations, the only remaining element of the list is equal to $k$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \leq n \leq 2\cdot 10^5$, $1 \leq k \leq 10^9$), the number of integers in the list, and the target value, respectively.</p><p>The second line of each test case contains the $n$ integers of the list $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases is not greater that $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if you can achieve $k$ with a sequence of $n-1$ operations. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (for example, "YES", "Yes", "yes", "yEs" will all be recognized as a positive answer).</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \leq n \leq 2\cdot 10^5$, $1 \leq k \leq 10^9$), the number of integers in the list, and the target value, respectively.</p><p>The second line of each test case contains the $n$ integers of the list $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases is not greater that $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if you can achieve $k$ with a sequence of $n-1$ operations. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (for example, "YES", "Yes", "yes", "yEs" will all be recognized as a positive answer).</p>





```input1
4
4 5
4 2 2 7
5 4
1 9 1 3 4
2 17
17 0
2 17
18 18
```




```output1
YES
NO
YES
NO
```



## Note

<p>In the first example we have the list $\{4, 2, 2, 7\}$, and we have the target $k = 5$. One way to achieve it is the following: first we choose the third element, obtaining the list $\{2, 0, 5\}$. Next we choose the first element, obtaining the list $\{-2, 3\}$. Finally, we choose the first element, obtaining the list $\{5\}$. </p>
