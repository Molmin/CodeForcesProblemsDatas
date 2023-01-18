## Description

<div><p>You are given a positive integer $n$.</p><p>Find a sequence of fractions $\frac{a_i}{b_i}$, $i = 1 \ldots k$ (where $a_i$ and $b_i$ are positive integers) for some $k$ such that:</p><p>$$ \begin{cases} \text{$b_i$ divides $n$, $1 &lt; b_i &lt; n$ for $i = 1 \ldots k$} \\ \text{$1 \le a_i &lt; b_i$ for $i = 1 \ldots k$} \\ \text{$\sum\limits_{i=1}^k \frac{a_i}{b_i} = 1 - \frac{1}{n}$} \end{cases} $$</p></div><div class="input-specification"><p>The input consists of a single integer $n$ ($2 \le n \le 10^9$).</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">YES</span>" if there exists such a sequence of fractions or "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>If there exists such a sequence, next lines should contain a description of the sequence in the following format.</p><p>The second line should contain integer $k$ ($1 \le k \le 100\,000$)&nbsp;— the number of elements in the sequence. It is guaranteed that if such a sequence exists, then there exists a sequence of length at most $100\,000$.</p><p>Next $k$ lines should contain fractions of the sequence with two integers $a_i$ and $b_i$ on each line.</p></div>

## Input

<p>The input consists of a single integer $n$ ($2 \le n \le 10^9$).</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">YES</span>" if there exists such a sequence of fractions or "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>If there exists such a sequence, next lines should contain a description of the sequence in the following format.</p><p>The second line should contain integer $k$ ($1 \le k \le 100\,000$)&nbsp;— the number of elements in the sequence. It is guaranteed that if such a sequence exists, then there exists a sequence of length at most $100\,000$.</p><p>Next $k$ lines should contain fractions of the sequence with two integers $a_i$ and $b_i$ on each line.</p>





```input1
2
```




```input2
6
```




```output1
NO
```




```output2
YES
2
1 2
1 3
```



## Note

<p>In the second example there is a sequence $\frac{1}{2}, \frac{1}{3}$ such that $\frac{1}{2} + \frac{1}{3} = 1 - \frac{1}{6}$.</p>
