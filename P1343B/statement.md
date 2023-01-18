## Description

<div><p>You are given a positive integer $n$, it is guaranteed that $n$ is even (i.e. divisible by $2$).</p><p>You want to construct the array $a$ of length $n$ such that: </p><ul> <li> The first $\frac{n}{2}$ elements of $a$ are even (divisible by $2$); </li><li> the second $\frac{n}{2}$ elements of $a$ are odd (not divisible by $2$); </li><li> <span class="tex-font-style-bf">all elements of $a$ are distinct and positive</span>; </li><li> the sum of the first half equals to the sum of the second half ($\sum\limits_{i=1}^{\frac{n}{2}} a_i = \sum\limits_{i=\frac{n}{2} + 1}^{n} a_i$). </li></ul><p>If there are multiple answers, you can print any. It is <span class="tex-font-style-bf">not guaranteed</span> that the answer exists.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of the array. It is guaranteed that that $n$ is even (i.e. divisible by $2$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer — "<span class="tex-font-style-tt">NO</span>" (without quotes), if there is no suitable answer for the given test case or "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-font-style-bf">any</span> suitable array $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) satisfying conditions from the problem statement on the second line.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of the array. It is guaranteed that that $n$ is even (i.e. divisible by $2$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer — "<span class="tex-font-style-tt">NO</span>" (without quotes), if there is no suitable answer for the given test case or "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-font-style-bf">any</span> suitable array $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) satisfying conditions from the problem statement on the second line.</p>





```input1
5
2
4
6
8
10
```




```output1
NO
YES
2 4 1 5
NO
YES
2 4 6 8 1 3 5 11
NO
```


