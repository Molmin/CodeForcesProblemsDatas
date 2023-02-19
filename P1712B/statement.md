## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">I wonder, does the falling rain</span></div></div> <div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">Forever yearn for it's disdain?</span></div><div class="epigraph-source">Effluvium of the Mind</div></div><p>You are given a positive integer $n$.</p><p>Find any permutation $p$ of length $n$ such that the sum $\operatorname{lcm}(1,p_1) + \operatorname{lcm}(2, p_2) + \ldots + \operatorname{lcm}(n, p_n)$ is as large as possible. </p><p>Here $\operatorname{lcm}(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple (LCM)</a> of integers $x$ and $y$.</p><p>A permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1\,000$). Description of the test cases follows.</p><p>The only line for each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print $n$ integers $p_1$, $p_2$, $\ldots$, $p_n$&nbsp;— the permutation with the maximum possible value of $\operatorname{lcm}(1,p_1) + \operatorname{lcm}(2, p_2) + \ldots + \operatorname{lcm}(n, p_n)$.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1\,000$). Description of the test cases follows.</p><p>The only line for each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print $n$ integers $p_1$, $p_2$, $\ldots$, $p_n$&nbsp;— the permutation with the maximum possible value of $\operatorname{lcm}(1,p_1) + \operatorname{lcm}(2, p_2) + \ldots + \operatorname{lcm}(n, p_n)$.</p><p>If there are multiple answers, print any of them.</p>





```input1|2
2
1
2
```




```output1
1 
2 1
```



## Note

<p>For $n = 1$, there is only one permutation, so the answer is $[1]$.</p><p>For $n = 2$, there are two permutations: </p><ul> <li> $[1, 2]$&nbsp;— the sum is $\operatorname{lcm}(1,1) + \operatorname{lcm}(2, 2) = 1 + 2 = 3$. </li><li> $[2, 1]$&nbsp;— the sum is $\operatorname{lcm}(1,2) + \operatorname{lcm}(2, 1) = 2 + 2 = 4$. </li></ul>
