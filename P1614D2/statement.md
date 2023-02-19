## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference is maximum value of $a_i$.</span></p><p>Once in <span class="tex-font-style-it">Kostomuksha</span> <span class="tex-font-style-it">Divan</span> found an array $a$ consisting of positive integers. Now he wants to reorder the elements of $a$ to maximize the value of the following function: $$\sum_{i=1}^n \operatorname{gcd}(a_1, \, a_2, \, \dots, \, a_i),$$ where $\operatorname{gcd}(x_1, x_2, \ldots, x_k)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> of integers $x_1, x_2, \ldots, x_k$, and $\operatorname{gcd}(x) = x$ for any integer $x$.</p><p>Reordering elements of an array means changing the order of elements in the array arbitrary, or leaving the initial order.</p><p>Of course, <span class="tex-font-style-it">Divan</span> can solve this problem. However, he found it interesting, so he decided to share it with you.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$) — the size of the array $a$.</p><p>The second line contains $n$ integers $a_{1}, \, a_{2}, \, \dots, \, a_{n}$ ($1 \le a_{i} \le 2 \cdot 10^7$) — the array $a$.</p></div><div class="output-specification"><p>Output the maximum value of the function that you can get by reordering elements of the array $a$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$) — the size of the array $a$.</p><p>The second line contains $n$ integers $a_{1}, \, a_{2}, \, \dots, \, a_{n}$ ($1 \le a_{i} \le 2 \cdot 10^7$) — the array $a$.</p>

## Output

<p>Output the maximum value of the function that you can get by reordering elements of the array $a$.</p>





```input1
6
2 3 1 2 6 2
```




```input2
10
5 7 10 3 1 10 100 3 42 54
```




```output1
14
```




```output2
131
```



## Note

<p>In the first example, it's optimal to rearrange the elements of the given array in the following order: $[6, \, 2, \, 2, \, 2, \, 3, \, 1]$:</p><p>$$\operatorname{gcd}(a_1) + \operatorname{gcd}(a_1, \, a_2) + \operatorname{gcd}(a_1, \, a_2, \, a_3) + \operatorname{gcd}(a_1, \, a_2, \, a_3, \, a_4) + \operatorname{gcd}(a_1, \, a_2, \, a_3, \, a_4, \, a_5) + \operatorname{gcd}(a_1, \, a_2, \, a_3, \, a_4, \, a_5, \, a_6) = 6 + 2 + 2 + 2 + 1 + 1 = 14.$$ It can be shown that it is impossible to get a better answer.</p><p>In the second example, it's optimal to rearrange the elements of a given array in the following order: $[100, \, 10, \, 10, \, 5, \, 1, \, 3, \, 3, \, 7, \, 42, \, 54]$.</p>
