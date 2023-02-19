## Description

<div><p>The $\text{$gcdSum$}$ of a positive integer is the $gcd$ of that integer with its sum of digits. Formally, $\text{$gcdSum$}(x) = gcd(x, \text{ sum of digits of } x)$ for a positive integer $x$. $gcd(a, b)$ denotes the greatest common divisor of $a$ and $b$ — the largest integer $d$ such that both integers $a$ and $b$ are divisible by $d$.</p><p>For example: $\text{$gcdSum$}(762) = gcd(762, 7 + 6 + 2)=gcd(762,15) = 3$.</p><p>Given an integer $n$, find the smallest integer $x \ge n$ such that $\text{$gcdSum$}(x) &gt; 1$.</p></div><div class="input-specification"><p>The first line of input contains one integer $t$ $(1 \le t \le 10^4)$ — the number of test cases. </p><p>Then $t$ lines follow, each containing a single integer $n$ $(1 \le n \le 10^{18})$.</p><p>All test cases in one test are different.</p></div><div class="output-specification"><p>Output $t$ lines, where the $i$-th line is a single integer containing the answer to the $i$-th test case.</p></div>

## Input

<p>The first line of input contains one integer $t$ $(1 \le t \le 10^4)$ — the number of test cases. </p><p>Then $t$ lines follow, each containing a single integer $n$ $(1 \le n \le 10^{18})$.</p><p>All test cases in one test are different.</p>

## Output

<p>Output $t$ lines, where the $i$-th line is a single integer containing the answer to the $i$-th test case.</p>





```input1
3
11
31
75
```




```output1
12
33
75
```



## Note

<p>Let us explain the three test cases in the sample.</p><p><span class="tex-font-style-bf">Test case 1:</span> $n = 11$: </p><p>$\text{$gcdSum$}(11) = gcd(11, 1 + 1) = gcd(11,\ 2) = 1$.</p><p>$\text{$gcdSum$}(12) = gcd(12, 1 + 2) = gcd(12,\ 3) = 3$.</p><p>So the smallest number $\ge 11$ whose $gcdSum$ $&gt; 1$ is $12$.</p><p><span class="tex-font-style-bf">Test case 2:</span> $n = 31$: </p><p>$\text{$gcdSum$}(31) = gcd(31, 3 + 1) = gcd(31,\ 4) = 1$.</p><p>$\text{$gcdSum$}(32) = gcd(32, 3 + 2) = gcd(32,\ 5) = 1$.</p><p>$\text{$gcdSum$}(33) = gcd(33, 3 + 3) = gcd(33,\ 6) = 3$.</p><p>So the smallest number $\ge 31$ whose $gcdSum$ $&gt; 1$ is $33$.</p><p><span class="tex-font-style-bf">Test case 3:</span> $\ n = 75$: </p><p>$\text{$gcdSum$}(75) = gcd(75, 7 + 5) = gcd(75,\ 12) = 3$.</p><p>The $\text{$gcdSum$}$ of $75$ is already $&gt; 1$. Hence, it is the answer.</p>
