## Description

<div><p>A sequence of integers $b_1, b_2, \ldots, b_m$ is called <span class="tex-font-style-it">good</span> if $max(b_1, b_2, \ldots, b_m) \cdot min(b_1, b_2, \ldots, b_m) \ge b_1 + b_2 + \ldots + b_m$.</p><p>A sequence of integers $a_1, a_2, \ldots, a_n$ is called <span class="tex-font-style-it">perfect</span> if every non-empty subsequence of $a$ is <span class="tex-font-style-it">good</span>.</p><p>YouKn0wWho has two integers $n$ and $M$, $M$ is prime. Help him find the number, modulo $M$, of <span class="tex-font-style-it">perfect</span> sequences $a_1, a_2, \ldots, a_n$ such that $1 \le a_i \le n + 1$ for each integer $i$ from $1$ to $n$.</p><p>A sequence $d$ is a subsequence of a sequence $c$ if $d$ can be obtained from $c$ by deletion of several (possibly, zero or all) elements.</p></div><div class="input-specification"><p>The first and only line of the input contains two space-separated integers $n$ and $M$ ($1 \le n \le 200$; $10^8 \le M \le 10^9$). It is guaranteed that <span class="tex-font-style-bf">$M$ is prime</span>.</p></div><div class="output-specification"><p>Print a single integer &nbsp;— the number of <span class="tex-font-style-it">perfect</span> sequences modulo $M$.</p></div>

## Input

<p>The first and only line of the input contains two space-separated integers $n$ and $M$ ($1 \le n \le 200$; $10^8 \le M \le 10^9$). It is guaranteed that <span class="tex-font-style-bf">$M$ is prime</span>.</p>

## Output

<p>Print a single integer &nbsp;— the number of <span class="tex-font-style-it">perfect</span> sequences modulo $M$.</p>





```input1
2 998244353
```




```input2
4 100000007
```




```input3
69 999999937
```




```output1
4
```




```output2
32
```




```output3
456886663
```



## Note

<p>In the first test case, the <span class="tex-font-style-it">perfect</span> sequences are $[2, 2]$, $[2, 3]$, $[3, 2]$ and $[3, 3]$.</p><p>In the second test case, some of the <span class="tex-font-style-it">perfect</span> sequences are $[3, 4, 3, 5]$, $[4, 5, 4, 4]$, $[4, 5, 5, 5]$ etc. One example of a sequence which is not <span class="tex-font-style-it">perfect</span> is $[2, 3, 3, 4]$, because, for example, the subsequence $[2, 3, 4]$ is not an <span class="tex-font-style-it">good</span> as $2 \cdot 4 &lt; 2 + 3 + 4$.</p>
