## Description

<div><p>You are given a string $s$ consisting of $n$ lowercase Latin letters.</p><p>Let's define a substring as a contiguous subsegment of a string. For example, "<span class="tex-font-style-tt">acab</span>" is a substring of "<span class="tex-font-style-tt">abacaba</span>" (it starts in position $3$ and ends in position $6$), but "<span class="tex-font-style-tt">aa</span>" or "<span class="tex-font-style-tt">d</span>" aren't substrings of this string. So the substring of the string $s$ from position $l$ to position $r$ is $s[l; r] = s_l s_{l + 1} \dots s_r$.</p><p>You have to choose <span class="tex-font-style-bf">exactly</span> one of the substrings of the given string and reverse it (i. e. make $s[l; r] = s_r s_{r - 1} \dots s_l$) to obtain a string that is <span class="tex-font-style-bf">less</span> lexicographically. Note that it <span class="tex-font-style-bf">is not necessary</span> to obtain the minimum possible string.</p><p>If it is impossible to reverse some substring of the given string to obtain a string that is less, print "<span class="tex-font-style-tt">NO</span>". Otherwise print "<span class="tex-font-style-tt">YES</span>" and <span class="tex-font-style-bf">any</span> suitable substring.</p><p>String $x$ is lexicographically less than string $y$, if either $x$ is a prefix of $y$ (and $x \ne y$), or there exists such $i$ ($1 \le i \le min(|x|, |y|)$), that $x_i &lt; y_i$, and for any $j$ ($1 \le j &lt; i$) $x_j = y_j$. Here $|a|$ denotes the length of the string $a$. The lexicographic comparison of strings is implemented by operator <span class="tex-font-style-tt">&lt;</span> in modern programming languages​​.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 3 \cdot 10^5$) — the length of $s$.</p><p>The second line of the input contains the string $s$ of length $n$ consisting only of lowercase Latin letters.</p></div><div class="output-specification"><p>If it is impossible to reverse some substring of the given string to obtain a string which is lexicographically <span class="tex-font-style-bf">less</span>, print "<span class="tex-font-style-tt">NO</span>". Otherwise print "<span class="tex-font-style-tt">YES</span>" and two indices $l$ and $r$ ($1 \le l &lt; r \le n$) denoting the substring you have to reverse. If there are multiple answers, you can print any.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 3 \cdot 10^5$) — the length of $s$.</p><p>The second line of the input contains the string $s$ of length $n$ consisting only of lowercase Latin letters.</p>

## Output

<p>If it is impossible to reverse some substring of the given string to obtain a string which is lexicographically <span class="tex-font-style-bf">less</span>, print "<span class="tex-font-style-tt">NO</span>". Otherwise print "<span class="tex-font-style-tt">YES</span>" and two indices $l$ and $r$ ($1 \le l &lt; r \le n$) denoting the substring you have to reverse. If there are multiple answers, you can print any.</p>





```input1
7
abacaba
```




```input2
6
aabcfg
```




```output1
YES
2 5
```




```output2
NO
```



## Note

<p>In the first testcase the resulting string is "<span class="tex-font-style-tt">aacabba</span>".</p>
