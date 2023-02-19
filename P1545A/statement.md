## Description

<div><p>AquaMoon has $n$ friends. They stand in a row from left to right, and the $i$-th friend from the left wears a T-shirt with a number $a_i$ written on it. Each friend has a direction (left or right). In the beginning, the direction of each friend is <span class="tex-font-style-bf">right</span>.</p><p>AquaMoon can make some operations on friends. On each operation, AquaMoon can choose two <span class="tex-font-style-bf">adjacent</span> friends and swap their positions. After each operation, the direction of both chosen friends will also be flipped: left to right and vice versa.</p><p>AquaMoon hopes that after some operations, the numbers written on the T-shirt of $n$ friends in the row, read from left to right, become <span class="tex-font-style-bf">non-decreasing</span>. Also she wants, that all friends will have a direction of <span class="tex-font-style-bf">right</span> at the end. Please find if it is possible.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 50$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$) — the number of Aquamoon's friends.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^5$) — the numbers, written on the T-shirts.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if there exists a possible sequence of operations, print "<span class="tex-font-style-tt">YES</span>" (without quotes); otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 50$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$) — the number of Aquamoon's friends.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^5$) — the numbers, written on the T-shirts.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, if there exists a possible sequence of operations, print "<span class="tex-font-style-tt">YES</span>" (without quotes); otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p>





```input1
3
4
4 3 2 5
4
3 3 2 2
5
1 2 3 5 4
```




```output1
YES
YES
NO
```



## Note

<p>The possible list of operations in the first test case:</p><ol> <li> Swap $a_1$ and $a_2$. The resulting sequence is $3, 4, 2, 5$. The directions are: left, left, right, right. </li><li> Swap $a_2$ and $a_3$. The resulting sequence is $3, 2, 4, 5$. The directions are: left, left, right, right. </li><li> Swap $a_1$ and $a_2$. The resulting sequence is $2, 3, 4, 5$. The directions are: right, right, right, right. </li></ol>
