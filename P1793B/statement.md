## Description

<div><p>For his birthday recently Fedya was given an array $a$ of $n$ integers arranged in a circle, For each pair of neighboring numbers ($a_1$ and $a_2$, $a_2$ and $a_3$, $\ldots$, $a_{n - 1}$ and $a_n$, $a_n$ and $a_1$) the absolute difference between them is equal to $1$.</p><p>Let's call a <span class="tex-font-style-it">local maximum</span> an element, which is greater than both of its neighboring elements. Also call a <span class="tex-font-style-it">local minimum</span> an element, which is less than both of its neighboring elements. Note, that elements $a_1$ and $a_n$ are neighboring elements.</p><p>Unfortunately, Fedya lost an array, but he remembered in it the sum of local maximums $x$ and the sum of local minimums $y$.</p><p>Given $x$ and $y$, help Fedya find any matching array of <span class="tex-font-style-bf">minimum</span> length.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>Each line of each test case contain two integers $x$ and $y$ ($-10^{9} \le y &lt; x \le 10^{9}$) — the sum of local maximums and the sum of local minimums, respectively.</p></div><div class="output-specification"><p>For each test case, in the first line print one integer $n$ — the minimum length of matching arrays.</p><p>In the second line print $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^{9} \leqslant a_i \leqslant 10^{9}$) — the array elements such that the the absolute difference between each pair of neighboring is equal to $1$.</p><p>If there are multiple solutions, print any of them.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^{5}$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>Each line of each test case contain two integers $x$ and $y$ ($-10^{9} \le y &lt; x \le 10^{9}$) — the sum of local maximums and the sum of local minimums, respectively.</p>

## Output

<p>For each test case, in the first line print one integer $n$ — the minimum length of matching arrays.</p><p>In the second line print $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^{9} \leqslant a_i \leqslant 10^{9}$) — the array elements such that the the absolute difference between each pair of neighboring is equal to $1$.</p><p>If there are multiple solutions, print any of them.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^{5}$.</p>





```input1|2,4
4
3 -2
4 -4
2 -1
5 -3
```




```output1
10
0 1 2 1 0 -1 0 -1 0 1
16
-2 -1 -2 -1 0 1 2 3 4 5 4 3 2 1 0 -1 
6
1 0 -1 0 1 0
16
2 3 2 1 0 -1 0 -1 0 -1 0 1 2 1 0 1
```



## Note

<p>In the first test case, the local maximums are the numbers at $3, 7$ and $10$ positions, and the local minimums are the numbers at $1, 6$ and $8$ positions. $x = a_3 + a_7 + a_{10} = 2 + 0 + 1 = 3$, $y = a_1 + a_6 + a_8 = 0 + (-1) + (-1) = -2$.</p><p>In the second test case, the local maximums are the numbers at $2$ and $10$ positions, and the local minimums are the numbers at $1$ and $3$ positions. $x = a_2 + a_{10} = -1 + 5 = 4$, $y = a_1 + a_3 = -2 + (-2) = -4$.</p><p>In the third test case, the local maximums are the numbers at $1$ and $5$ positions, and the local minimums are the numbers at $3$ and $6$ positions.</p>
