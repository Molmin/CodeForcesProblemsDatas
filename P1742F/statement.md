## Description

<div><p>Alperen has two strings, $s$ and $t$ which are both initially equal to "<span class="tex-font-style-tt">a</span>". </p><p>He will perform $q$ operations of two types on the given strings:</p><ul> <li> $1 \;\; k \;\; x$ — Append the string $x$ exactly $k$ times at the end of string $s$. In other words, $s := s + \underbrace{x + \dots + x}_{k \text{ times}}$. </li><li> $2 \;\; k \;\; x$ — Append the string $x$ exactly $k$ times at the end of string $t$. In other words, $t := t + \underbrace{x + \dots + x}_{k \text{ times}}$. </li></ul><p>After each operation, determine if it is possible to <span class="tex-font-style-bf">rearrange</span> the characters of $s$ and $t$ such that $s$ is lexicographically smaller$^{\dagger}$ than $t$.</p><p>Note that the strings change after performing each operation and <span class="tex-font-style-bf">don't</span> go back to their initial states.</p><p>$^{\dagger}$ Simply speaking, the lexicographical order is the order in which words are listed in a dictionary. A formal definition is as follows: string $p$ is lexicographically smaller than string $q$ if there exists a position $i$ such that $p_i &lt; q_i$, and for all $j &lt; i$, $p_j = q_j$. If no such $i$ exists, then $p$ is lexicographically smaller than $q$ if the length of $p$ is less than the length of $q$. For example, $\texttt{abdc} &lt; \texttt{abe}$ and $\texttt{abc} &lt; \texttt{abcd}$, where we write $p &lt; q$ if $p$ is lexicographically smaller than $q$.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $q$ $(1 \leq q \leq 10^5)$&nbsp;— the number of operations Alperen will perform.</p><p>Then $q$ lines follow, each containing two positive integers $d$ and $k$ ($1 \leq d \leq 2$; $1 \leq k \leq 10^5$) and a non-empty string $x$ consisting of lowercase English letters — the type of the operation, the number of times we will append string $x$ and the string we need to append respectively.</p><p>It is guaranteed that the sum of $q$ over all test cases doesn't exceed $10^5$ and that the sum of lengths of all strings $x$ in the input doesn't exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each operation, output "<span class="tex-font-style-tt">YES</span>", if it is possible to arrange the elements in both strings in such a way that $s$ is lexicographically smaller than $t$ and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $q$ $(1 \leq q \leq 10^5)$&nbsp;— the number of operations Alperen will perform.</p><p>Then $q$ lines follow, each containing two positive integers $d$ and $k$ ($1 \leq d \leq 2$; $1 \leq k \leq 10^5$) and a non-empty string $x$ consisting of lowercase English letters — the type of the operation, the number of times we will append string $x$ and the string we need to append respectively.</p><p>It is guaranteed that the sum of $q$ over all test cases doesn't exceed $10^5$ and that the sum of lengths of all strings $x$ in the input doesn't exceed $5 \cdot 10^5$.</p>

## Output

<p>For each operation, output "<span class="tex-font-style-tt">YES</span>", if it is possible to arrange the elements in both strings in such a way that $s$ is lexicographically smaller than $t$ and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1|2,3,4,5,6,7,11,12,13,14
3
5
2 1 aa
1 2 a
2 3 a
1 2 b
2 3 abca
2
1 5 mihai
2 2 buiucani
3
1 5 b
2 3 a
2 4 paiu
```




```output1
YES
NO
YES
NO
YES
NO
YES
NO
NO
YES
```



## Note

<p>In the first test case, the strings are initially $s = $ "<span class="tex-font-style-tt">a</span>" and $t = $ "<span class="tex-font-style-tt">a</span>". </p><p>After the first operation the string $t$ becomes "<span class="tex-font-style-tt">aaa</span>". Since "<span class="tex-font-style-tt">a</span>" is already lexicographically smaller than "<span class="tex-font-style-tt">aaa</span>", the answer for this operation should be "<span class="tex-font-style-tt">YES</span>".</p><p>After the second operation string $s$ becomes "<span class="tex-font-style-tt">aaa</span>", and since $t$ is also equal to "<span class="tex-font-style-tt">aaa</span>", we can't arrange $s$ in any way such that it is lexicographically smaller than $t$, so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>After the third operation string $t$ becomes "<span class="tex-font-style-tt">aaaaaa</span>" and $s$ is already lexicographically smaller than it so the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>After the fourth operation $s$ becomes "<span class="tex-font-style-tt">aaabb</span>" and there is no way to make it lexicographically smaller than "<span class="tex-font-style-tt">aaaaaa</span>" so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>After the fifth operation the string $t$ becomes "<span class="tex-font-style-tt">aaaaaaabcaabcaabca</span>", and we can rearrange the strings to: "<span class="tex-font-style-tt">bbaaa</span>" and "<span class="tex-font-style-tt">caaaaaabcaabcaabaa</span>" so that $s$ is lexicographically smaller than $t$, so we should answer "<span class="tex-font-style-tt">YES</span>". </p>
