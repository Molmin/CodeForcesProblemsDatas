## Description

<div><p>Vasya has a multiset $s$ consisting of $n$ integer numbers. Vasya calls some number $x$ nice if it appears in the multiset exactly once. For example, multiset $\{1, 1, 2, 3, 3, 3, 4\}$ contains nice numbers $2$ and $4$.</p><p>Vasya wants to split multiset $s$ into two multisets $a$ and $b$ <span class="tex-font-style-bf">(one of which may be empty)</span> in such a way that the quantity of nice numbers in multiset $a$ would be the same as the quantity of nice numbers in multiset $b$ (the quantity of numbers to appear exactly once in multiset $a$ and the quantity of numbers to appear exactly once in multiset $b$).</p></div><div class="input-specification"><p>The first line contains a single integer $n~(2 \le n \le 100)$.</p><p>The second line contains $n$ integers $s_1, s_2, \dots s_n~(1 \le s_i \le 100)$ — the multiset $s$.</p></div><div class="output-specification"><p>If there exists no split of $s$ to satisfy the given requirements, then print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line.</p><p>The second line should contain a string, consisting of $n$ characters. $i$-th character should be equal to '<span class="tex-font-style-tt">A</span>' if the $i$-th element of multiset $s$ goes to multiset $a$ and '<span class="tex-font-style-tt">B</span>' if if the $i$-th element of multiset $s$ goes to multiset $b$. <span class="tex-font-style-bf">Elements are numbered from $1$ to $n$ in the order they are given in the input.</span></p><p>If there exist multiple solutions, then print any of them.</p></div>

## Input

<p>The first line contains a single integer $n~(2 \le n \le 100)$.</p><p>The second line contains $n$ integers $s_1, s_2, \dots s_n~(1 \le s_i \le 100)$ — the multiset $s$.</p>

## Output

<p>If there exists no split of $s$ to satisfy the given requirements, then print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line.</p><p>The second line should contain a string, consisting of $n$ characters. $i$-th character should be equal to '<span class="tex-font-style-tt">A</span>' if the $i$-th element of multiset $s$ goes to multiset $a$ and '<span class="tex-font-style-tt">B</span>' if if the $i$-th element of multiset $s$ goes to multiset $b$. <span class="tex-font-style-bf">Elements are numbered from $1$ to $n$ in the order they are given in the input.</span></p><p>If there exist multiple solutions, then print any of them.</p>





```input1
4
3 5 7 1

```




```input2
3
3 5 1

```




```output1
YES
BABA

```




```output2
NO

```


