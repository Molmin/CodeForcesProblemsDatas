## Description

<div><p>You are given a sequence $s$ consisting of $n$ digits from $1$ to $9$.</p><p>You have to divide it into <span class="tex-font-style-bf">at least two</span> segments (segment — is a consecutive sequence of elements) (in other words, you have to place separators between some digits of the sequence) in such a way that <span class="tex-font-style-bf">each element belongs to exactly one segment</span> and if the resulting division will be represented as an integer numbers sequence then each next element of this sequence will be <span class="tex-font-style-bf">strictly greater</span> than the previous one.</p><p>More formally: if the resulting division of the sequence is $t_1, t_2, \dots, t_k$, where $k$ is the number of element in a division, then for each $i$ from $1$ to $k-1$ the condition $t_{i} &lt; t_{i + 1}$ (using <span class="tex-font-style-bf">numerical</span> comparing, it means that the integer representations of strings are compared) should be satisfied.</p><p>For example, if $s=654$ then you can divide it into parts $[6, 54]$ and it will be suitable division. But if you will divide it into parts $[65, 4]$ then it will be bad division because $65 &gt; 4$. If $s=123$ then you can divide it into parts $[1, 23]$, $[1, 2, 3]$ but not into parts $[12, 3]$.</p><p>Your task is to find <span class="tex-font-style-bf">any</span> suitable division for each of the $q$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 300$) — the number of queries.</p><p>The first line of the $i$-th query contains one integer number $n_i$ ($2 \le n_i \le 300$) — the number of digits in the $i$-th query.</p><p>The second line of the $i$-th query contains one string $s_i$ of length $n_i$ consisting only of digits from $1$ to $9$.</p></div><div class="output-specification"><p>If the sequence of digits in the $i$-th query cannot be divided into <span class="tex-font-style-bf">at least two</span> parts in a way described in the problem statement, print the single line "<span class="tex-font-style-tt">NO</span>" for this query.</p><p>Otherwise in the first line of the answer to this query print "<span class="tex-font-style-tt">YES</span>", on the second line print $k_i$ — the number of parts in your division of the $i$-th query sequence and in the third line print $k_i$ strings $t_{i, 1}, t_{i, 2}, \dots, t_{i, k_i}$ — your division. Parts should be printed in order of the initial string digits. It means that if you write the parts one after another without changing their order then you'll get the string $s_i$.</p><p>See examples for better understanding.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 300$) — the number of queries.</p><p>The first line of the $i$-th query contains one integer number $n_i$ ($2 \le n_i \le 300$) — the number of digits in the $i$-th query.</p><p>The second line of the $i$-th query contains one string $s_i$ of length $n_i$ consisting only of digits from $1$ to $9$.</p>

## Output

<p>If the sequence of digits in the $i$-th query cannot be divided into <span class="tex-font-style-bf">at least two</span> parts in a way described in the problem statement, print the single line "<span class="tex-font-style-tt">NO</span>" for this query.</p><p>Otherwise in the first line of the answer to this query print "<span class="tex-font-style-tt">YES</span>", on the second line print $k_i$ — the number of parts in your division of the $i$-th query sequence and in the third line print $k_i$ strings $t_{i, 1}, t_{i, 2}, \dots, t_{i, k_i}$ — your division. Parts should be printed in order of the initial string digits. It means that if you write the parts one after another without changing their order then you'll get the string $s_i$.</p><p>See examples for better understanding.</p>





```input1
4
6
654321
4
1337
2
33
4
2122
```




```output1
YES
3
6 54 321
YES
3
1 3 37
NO
YES
2
21 22
```


