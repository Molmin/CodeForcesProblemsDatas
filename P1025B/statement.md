## Description

<div><p>During the research on properties of the greatest common divisor (<span class="tex-font-style-it">GCD</span>) of a set of numbers, Ildar, a famous mathematician, introduced a brand new concept of the weakened common divisor (<span class="tex-font-style-it">WCD</span>) of a list of pairs of integers.</p><p>For a given list of pairs of integers $(a_1, b_1)$, $(a_2, b_2)$, ..., $(a_n, b_n)$ their <span class="tex-font-style-it">WCD</span> is arbitrary integer greater than $1$, such that it divides at least one element in each pair. WCD may not exist for some lists.</p><p>For example, if the list looks like $[(12, 15), (25, 18), (10, 24)]$, then their WCD can be equal to $2$, $3$, $5$ or $6$ (each of these numbers is strictly greater than $1$ and divides at least one number in each pair).</p><p>You're currently pursuing your PhD degree under Ildar's mentorship, and that's why this problem was delegated to you. Your task is to calculate <span class="tex-font-style-it">WCD</span> efficiently.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 150\,000$)&nbsp;— the number of pairs.</p><p>Each of the next $n$ lines contains two integer values $a_i$, $b_i$ ($2 \le a_i, b_i \le 2 \cdot 10^9$).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the <span class="tex-font-style-it">WCD</span> of the set of pairs. </p><p>If there are multiple possible answers, output any; if there is no answer, print $-1$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 150\,000$)&nbsp;— the number of pairs.</p><p>Each of the next $n$ lines contains two integer values $a_i$, $b_i$ ($2 \le a_i, b_i \le 2 \cdot 10^9$).</p>

## Output

<p>Print a single integer&nbsp;— the <span class="tex-font-style-it">WCD</span> of the set of pairs. </p><p>If there are multiple possible answers, output any; if there is no answer, print $-1$.</p>





```input1
3
17 18
15 24
12 15

```




```input2
2
10 16
7 17

```




```input3
5
90 108
45 105
75 40
165 175
33 30

```




```output1
6
```




```output2
-1

```




```output3
5

```



## Note

<p>In the first example the answer is $6$ since it divides $18$ from the first pair, $24$ from the second and $12$ from the third ones. Note that other valid answers will also be accepted.</p><p>In the second example there are no integers greater than $1$ satisfying the conditions.</p><p>In the third example one of the possible answers is $5$. Note that, for example, $15$ is also allowed, but it's not necessary to maximize the output.</p>
