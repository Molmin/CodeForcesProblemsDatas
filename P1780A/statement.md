## Description

<div><p>Today Hayato came home from school with homework.</p><p>In the assignment, Hayato was given an array $a$ of length $n$. The task was to find $3$ numbers in this array whose sum is <span class="tex-font-style-bf">odd</span>. At school, he claimed that there are such $3$ numbers, but Hayato was not sure, so he asked you for help.</p><p>Answer if there are such three numbers, and if so, output indices $i$, $j$, and $k$ such that $a_i + a_j + a_k$ is odd.</p><p>The odd numbers are integers that are not divisible by $2$: $1$, $3$, $5$, and so on.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>For each test case, the first line contains one integer $n$ ($3 \le n \le 300$) — the length of $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^5$) — the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, in the first line print one word "<span class="tex-font-style-tt">YES</span>" (without quotes) if there are $3$ numbers with an odd sum or "<span class="tex-font-style-tt">NO</span>" (without quotes) if there are no such $3$ numbers.</p><p>If the answer exists, then on the second line print $3$ distinct integers $i, j, k$ ($1 \le i, j, k \le n$) — the indices of the numbers. If there are several answers, output any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>For each test case, the first line contains one integer $n$ ($3 \le n \le 300$) — the length of $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^5$) — the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, in the first line print one word "<span class="tex-font-style-tt">YES</span>" (without quotes) if there are $3$ numbers with an odd sum or "<span class="tex-font-style-tt">NO</span>" (without quotes) if there are no such $3$ numbers.</p><p>If the answer exists, then on the second line print $3$ distinct integers $i, j, k$ ($1 \le i, j, k \le n$) — the indices of the numbers. If there are several answers, output any.</p>





```input1|2,3,6,7,10,11
6
3
1 1 1
4
1 1 2 2
3
1 2 3
5
1 4 5 1 2
4
2 6 2 4
5
5 6 3 2 1
```




```output1
YES
1 2 3
YES
3 4 1
NO
YES
1 3 4
NO
YES
1 3 5
```



## Note

<p>In the first test case, there is one way to choose $3$ numbers, and since $1 + 1 + 1 = 3$, this triple is fine for us.</p><p>In the second test case, you need to choose the numbers $1, 2, 2$, since $1 + 2 + 2 = 5$.</p><p>In the third test case, there is one way to choose three numbers, but $1 + 2 + 3 = 6$ is an even number, so the required triple does not exist.</p><p>In the fifth test case, no matter what three numbers we choose, their sum is even.</p>
