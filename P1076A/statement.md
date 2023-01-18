## Description

<div><p>You are given a string $s$ consisting of $n$ lowercase Latin letters.</p><p>You have to remove <span class="tex-font-style-bf">at most one</span> (i.e. zero or one) character of this string in such a way that the string you obtain will be lexicographically smallest among all strings that can be obtained using this operation.</p><p>String $s = s_1 s_2 \dots s_n$ is <span class="tex-font-style-it">lexicographically smaller</span> than string $t = t_1 t_2 \dots t_m$ if $n &lt; m$ and $s_1 = t_1, s_2 = t_2, \dots, s_n = t_n$ or there exists a number $p$ such that $p \le min(n, m)$ and $s_1 = t_1, s_2 = t_2, \dots, s_{p-1} = t_{p-1}$ and $s_p &lt; t_p$.</p><p>For example, "<span class="tex-font-style-tt">aaa</span>" is smaller than "<span class="tex-font-style-tt">aaaa</span>", "<span class="tex-font-style-tt">abb</span>" is smaller than "<span class="tex-font-style-tt">abc</span>", "<span class="tex-font-style-tt">pqr</span>" is smaller than "<span class="tex-font-style-tt">z</span>".</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of $s$.</p><p>The second line of the input contains exactly $n$ lowercase Latin letters — the string $s$.</p></div><div class="output-specification"><p>Print one string — the smallest possible lexicographically string that can be obtained by removing <span class="tex-font-style-bf">at most one</span> character from the string $s$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of $s$.</p><p>The second line of the input contains exactly $n$ lowercase Latin letters — the string $s$.</p>

## Output

<p>Print one string — the smallest possible lexicographically string that can be obtained by removing <span class="tex-font-style-bf">at most one</span> character from the string $s$.</p>





```input1
3
aaa
```




```input2
5
abcda
```




```output1
aa
```




```output2
abca
```



## Note

<p>In the first example you can remove any character of $s$ to obtain the string "<span class="tex-font-style-tt">aa</span>".</p><p>In the second example "<span class="tex-font-style-tt">abca</span>" &lt; "<span class="tex-font-style-tt">abcd</span>" &lt; "<span class="tex-font-style-tt">abcda</span>" &lt; "<span class="tex-font-style-tt">abda</span>" &lt; "<span class="tex-font-style-tt">acda</span>" &lt; "<span class="tex-font-style-tt">bcda</span>".</p>
