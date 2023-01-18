## Description

<div><p>Mr. F has $n$ positive integers, $a_1, a_2, \ldots, a_n$.</p><p>He thinks the greatest common divisor of these integers is too small. So he wants to enlarge it by removing some of the integers.</p><p>But this problem is too simple for him, so he does not want to do it by himself. If you help him, he will give you some scores in reward.</p><p>Your task is to calculate the minimum number of integers you need to remove so that the greatest common divisor of the remaining integers is bigger than that of all integers.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \leq n \leq 3 \cdot 10^5$) — the number of integers Mr. F has.</p><p>The second line contains $n$ integers, $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 1.5 \cdot 10^7$).</p></div><div class="output-specification"><p>Print an integer&nbsp;— the minimum number of integers you need to remove so that the greatest common divisor of the remaining integers is bigger than that of all integers.</p><p>You should not remove all of the integers.</p><p>If there is no solution, print «<span class="tex-font-style-tt">-1</span>» (without quotes).</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \leq n \leq 3 \cdot 10^5$) — the number of integers Mr. F has.</p><p>The second line contains $n$ integers, $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 1.5 \cdot 10^7$).</p>

## Output

<p>Print an integer&nbsp;— the minimum number of integers you need to remove so that the greatest common divisor of the remaining integers is bigger than that of all integers.</p><p>You should not remove all of the integers.</p><p>If there is no solution, print «<span class="tex-font-style-tt">-1</span>» (without quotes).</p>





```input1
3
1 2 4

```




```input2
4
6 9 15 30

```




```input3
3
1 1 1

```




```output1
1
```




```output2
2
```




```output3
-1
```



## Note

<p>In the first example, the greatest common divisor is $1$ in the beginning. You can remove $1$ so that the greatest common divisor is enlarged to $2$. The answer is $1$.</p><p>In the second example, the greatest common divisor is $3$ in the beginning. You can remove $6$ and $9$ so that the greatest common divisor is enlarged to $15$. There is no solution which removes only one integer. So the answer is $2$.</p><p>In the third example, there is no solution to enlarge the greatest common divisor. So the answer is $-1$.</p>
