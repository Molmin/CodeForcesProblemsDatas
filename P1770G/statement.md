## Description

<div><p>Chiyuu has a bracket sequence$^\dagger$ $s$ of length $n$. Let $k$ be the minimum number of characters that Chiyuu has to remove from $s$ to make $s$ balanced$^\ddagger$.</p><p>Now, Koxia wants you to count the number of ways to remove $k$ characters from $s$ so that $s$ becomes balanced, modulo $998\,244\,353$.</p><p>Note that two ways of removing characters are considered distinct if and only if the set of indices removed is different.</p><p>$^\dagger$ A bracket sequence is a string containing only the characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p><p>$^\ddagger$ A bracket sequence is called balanced if one can turn it into a valid math expression by adding characters <span class="tex-font-style-tt">+</span> and <span class="tex-font-style-tt">1</span>. For example, sequences <span class="tex-font-style-tt">(())()</span>, <span class="tex-font-style-tt">()</span>, <span class="tex-font-style-tt">(()(()))</span> and the empty string are balanced, while <span class="tex-font-style-tt">)(</span>, <span class="tex-font-style-tt">(()</span>, and <span class="tex-font-style-tt">(()))(</span> are not.</p></div><div class="input-specification"><p>The first line of input contains a string $s$ ($1 \leq |s| \leq 5 \cdot {10}^5$) — the bracket sequence.</p><p>It is guaranteed that $s$ only contains the characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p></div><div class="output-specification"><p>Output a single integer — the number of ways to remove $k$ characters from $s$ so that $s$ becomes balanced, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line of input contains a string $s$ ($1 \leq |s| \leq 5 \cdot {10}^5$) — the bracket sequence.</p><p>It is guaranteed that $s$ only contains the characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p>

## Output

<p>Output a single integer — the number of ways to remove $k$ characters from $s$ so that $s$ becomes balanced, modulo $998\,244\,353$.</p>





```input1
())(()
```




```input2
(
```




```output1
4
```




```output2
1
```



## Note

<p>In the first test case, it can be proved that the minimum number of characters that Chiyuu has to remove is $2$. There are $4$ ways to remove $2$ characters to make $s$ balanced as follows. Deleted characters are noted as red.</p><ul> <li> $\texttt{(} \color{Red}{\texttt{)}} \texttt{)} \color{Red}{\texttt{(}} \texttt{(} \texttt{)}$, </li><li> $\texttt{(} \texttt{)} \color{Red}{\texttt{)}} \color{Red}{\texttt{(}} \texttt{(} \texttt{)}$, </li><li> $\texttt{(} \color{Red}{\texttt{)}} \texttt{)} \texttt{(} \color{Red}{\texttt{(}} \texttt{)}$, </li><li> $\texttt{(} \texttt{)} \color{Red}{\texttt{)}} \texttt{(} \color{Red}{\texttt{(}} \texttt{)}$. </li></ul><p>In the second test case, the only way to make $s$ balanced is by deleting the only character to get an empty bracket sequence, which is considered balanced.</p>
