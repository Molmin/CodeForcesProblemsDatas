## Description

<div><p>Daemon Targaryen decided to stop looking like a Metin2 character. He turned himself into the most beautiful thing, a bracket sequence.</p><p>For a bracket sequence, we can do two kind of operations:</p><ul> <li> Select one of its substrings$^\dagger$ and cyclic shift it to the right. For example, after a cyclic shift to the right, "<span class="tex-font-style-tt">(())</span>" will become "<span class="tex-font-style-tt">)(()</span>"; </li><li> Insert any bracket, opening '<span class="tex-font-style-tt">(</span>' or closing '<span class="tex-font-style-tt">)</span>', wherever you want in the sequence. </li></ul><p>We define the <span class="tex-font-style-it">cost</span> of a bracket sequence as the <span class="tex-font-style-bf">minimum</span> number of such operations to make it balanced$^\ddagger$.</p><p>Given a bracket sequence $s$ of length $n$, find the sum of costs across all its $\frac{n(n+1)}{2}$ non-empty substrings. Note that for each substring we calculate the cost <span class="tex-font-style-bf">independently</span>.</p><p>$^\dagger$ A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p><p>$^\ddagger$ A sequence of brackets is called balanced if one can turn it into a valid math expression by adding characters $+$ and $1$. For example, sequences "<span class="tex-font-style-tt">(())()</span>", "<span class="tex-font-style-tt">()</span>", and "<span class="tex-font-style-tt">(()(()))</span>" are balanced, while "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(()</span>", and "<span class="tex-font-style-tt">(()))(</span>" are not.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the bracket sequence.</p><p>The second line of each test case contains a string $s$, consisting only of characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>', of length $n$ — the bracket sequence.</p><p>It is guaranteed that sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer — the sum of costs of all substrings of $s$.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the bracket sequence.</p><p>The second line of each test case contains a string $s$, consisting only of characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>', of length $n$ — the bracket sequence.</p><p>It is guaranteed that sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer — the sum of costs of all substrings of $s$.</p>





```input1|2,3,6,7,10,11
5
1
)
4
)()(
3
())
5
(((((
10
)(())))())
```




```output1
1
9
6
35
112
```



## Note

<p>In the first test case, there is the only substring "<span class="tex-font-style-tt">)</span>". Its cost is $1$ because we can insert '<span class="tex-font-style-tt">(</span>' to the beginning of this substring and get a string "<span class="tex-font-style-tt">()</span>", that is a balanced string.</p><p>In the second test case, the cost of each substring of length one is $1$. The cost of a substring "<span class="tex-font-style-tt">)(</span>" is $1$ because we can cyclically shift it to right and get a string "<span class="tex-font-style-tt">()</span>". The cost of strings "<span class="tex-font-style-tt">)()</span>" and "<span class="tex-font-style-tt">()(</span>" is $1$ because its enough to insert one bracket to each of them. The cost of substring "<span class="tex-font-style-tt">)()(</span>" is $1$ because we can cyclically shift it to right and get a string "<span class="tex-font-style-tt">()()</span>". So there are $4 + 2 + 2 + 1 = 9$ substring of cost $1$ and $1$ substring of cost $0$. So the sum of the costs is $9$.</p><p>In the third test case, </p><ul> <li> "<span class="tex-font-style-tt">(</span>", the cost is $1$; </li><li> "<span class="tex-font-style-tt">()</span>", the cost is $0$; </li><li> "<span class="tex-font-style-tt">())</span>", the cost is $1$; </li><li> "<span class="tex-font-style-tt">)</span>", the cost is $1$; </li><li> "<span class="tex-font-style-tt">))</span>", the cost is $2$; </li><li> "<span class="tex-font-style-tt">)</span>", the cost is $1$. </li></ul><p>So the sum of the costs is $6$.</p>
