## Description

<div><p><span class="tex-font-style-bf">This is a harder version of the problem with bigger constraints.</span></p><p>Korney Korneevich dag up an array $a$ of length $n$. Korney Korneevich has recently read about the operation <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a>, so he wished to experiment with it. For this purpose, he decided to find all integers $x \ge 0$ such that there exists an <span class="tex-font-style-bf">increasing</span> subsequence of the array $a$, in which the bitwise XOR of numbers is equal to $x$.</p><p>It didn't take a long time for Korney Korneevich to find all such $x$, and he wants to check his result. That's why he asked you to solve this problem!</p><p>A sequence $s$ is a subsequence of a sequence $b$ if $s$ can be obtained from $b$ by deletion of several (possibly, zero or all) elements.</p><p>A sequence $s_1, s_2, \ldots , s_m$ is called increasing if $s_1 &lt; s_2 &lt; \ldots &lt; s_m$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^6$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 5000$) — the elements of the array $a$.</p></div><div class="output-specification"><p>In the first line print a single integer $k$ — the number of found $x$ values.</p><p>In the second line print $k$ integers in <span class="tex-font-style-bf">increasing</span> order $x_1, x_2, \ldots x_k$ ($0 \le x_1 &lt; \ldots &lt; x_k$) — found $x$ values.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^6$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 5000$) — the elements of the array $a$.</p>

## Output

<p>In the first line print a single integer $k$ — the number of found $x$ values.</p><p>In the second line print $k$ integers in <span class="tex-font-style-bf">increasing</span> order $x_1, x_2, \ldots x_k$ ($0 \le x_1 &lt; \ldots &lt; x_k$) — found $x$ values.</p>





```input1
4
4 2 2 4
```




```input2
8
1 0 1 7 12 5 3 2
```




```output1
4
0 2 4 6
```




```output2
12
0 1 2 3 4 5 6 7 10 11 12 13
```



## Note

<p>In the first test case:</p><ul> <li> To get value $x = 0$ it is possible to choose and empty subsequence </li><li> To get value $x = 2$ it is possible to choose a subsequence $[2]$ </li><li> To get value $x = 4$ it is possible to choose a subsequence $[4]$ </li><li> To get value $x = 6$ it is possible to choose a subsequence $[2, 4]$ </li></ul>
