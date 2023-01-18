## Description

<div><p>You are given a string $t$ and $n$ strings $s_1, s_2, \dots, s_n$. All strings consist of lowercase Latin letters.</p><p>Let $f(t, s)$ be the number of occurences of string $s$ in string $t$. For example, $f('\text{aaabacaa}', '\text{aa}') = 3$, and $f('\text{ababa}', '\text{aba}') = 2$.</p><p>Calculate the value of $\sum\limits_{i=1}^{n} \sum\limits_{j=1}^{n} f(t, s_i + s_j)$, where $s + t$ is the concatenation of strings $s$ and $t$. Note that if there are two pairs $i_1$, $j_1$ and $i_2$, $j_2$ such that $s_{i_1} + s_{j_1} = s_{i_2} + s_{j_2}$, you should include both $f(t, s_{i_1} + s_{j_1})$ and $f(t, s_{i_2} + s_{j_2})$ in answer.</p></div><div class="input-specification"><p>The first line contains string $t$ ($1 \le |t| \le 2 \cdot 10^5$).</p><p>The second line contains integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>Each of next $n$ lines contains string $s_i$ ($1 \le |s_i| \le 2 \cdot 10^5$).</p><p>It is guaranteed that $\sum\limits_{i=1}^{n} |s_i| \le 2 \cdot 10^5$. All strings consist of lowercase English letters.</p></div><div class="output-specification"><p>Print one integer — the value of $\sum\limits_{i=1}^{n} \sum\limits_{j=1}^{n} f(t, s_i + s_j)$.</p></div>

## Input

<p>The first line contains string $t$ ($1 \le |t| \le 2 \cdot 10^5$).</p><p>The second line contains integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>Each of next $n$ lines contains string $s_i$ ($1 \le |s_i| \le 2 \cdot 10^5$).</p><p>It is guaranteed that $\sum\limits_{i=1}^{n} |s_i| \le 2 \cdot 10^5$. All strings consist of lowercase English letters.</p>

## Output

<p>Print one integer — the value of $\sum\limits_{i=1}^{n} \sum\limits_{j=1}^{n} f(t, s_i + s_j)$.</p>





```input1
aaabacaa
2
a
aa
```




```input2
aaabacaa
4
a
a
a
b
```




```output1
5
```




```output2
33
```


