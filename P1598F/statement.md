## Description

<div><p>A bracket sequence is a string containing only characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>". A regular bracket sequence (or, shortly, an RBS) is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">+</span>" between the original characters of the sequence. For example:</p><ul> <li> bracket sequences "<span class="tex-font-style-tt">()()</span>" and "<span class="tex-font-style-tt">(())</span>" are regular (the resulting expressions are: "<span class="tex-font-style-tt">(1)+(1)</span>" and "<span class="tex-font-style-tt">((1+1)+1)</span>"); </li><li> bracket sequences "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" are not. </li></ul><p>Let's denote the concatenation of two strings $x$ and $y$ as $x+y$. For example, "<span class="tex-font-style-tt">()()</span>"&nbsp;$+$&nbsp;"<span class="tex-font-style-tt">)(</span>"&nbsp;$=$&nbsp;"<span class="tex-font-style-tt">()())(</span>".</p><p>You are given $n$ bracket sequences $s_1, s_2, \dots, s_n$. You can rearrange them in any order (you can rearrange only the strings themselves, but not the characters in them).</p><p>Your task is to rearrange the strings in such a way that the string $s_1 + s_2 + \dots + s_n$ has as many non-empty prefixes that are RBS as possible.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 20$).</p><p>Then $n$ lines follow, the $i$-th of them contains $s_i$&nbsp;— a bracket sequence (a string consisting of characters "<span class="tex-font-style-tt">(</span>" and/or "<span class="tex-font-style-tt">)</span>". All sequences $s_i$ are non-empty, their total length does not exceed $4 \cdot 10^5$.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the maximum number of non-empty prefixes that are RBS for the string $s_1 + s_2 + \dots + s_n$, if the strings $s_1, s_2, \dots, s_n$ can be rearranged arbitrarily.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 20$).</p><p>Then $n$ lines follow, the $i$-th of them contains $s_i$&nbsp;— a bracket sequence (a string consisting of characters "<span class="tex-font-style-tt">(</span>" and/or "<span class="tex-font-style-tt">)</span>". All sequences $s_i$ are non-empty, their total length does not exceed $4 \cdot 10^5$.</p>

## Output

<p>Print one integer&nbsp;— the maximum number of non-empty prefixes that are RBS for the string $s_1 + s_2 + \dots + s_n$, if the strings $s_1, s_2, \dots, s_n$ can be rearranged arbitrarily.</p>





```input1
2
(
)
```




```input2
4
()()())
(
(
)
```




```input3
1
(())
```




```input4
1
)(()
```




```output1
1
```




```output2
4
```




```output3
1
```




```output4
0
```



## Note

<p>In the first example, you can concatenate the strings as follows: "<span class="tex-font-style-tt">(</span>"&nbsp;$+$&nbsp;"<span class="tex-font-style-tt">)</span>"&nbsp;$=$&nbsp;"<span class="tex-font-style-tt">()</span>", the resulting string will have one prefix, that is an RBS: "<span class="tex-font-style-tt">()</span>".</p><p>In the second example, you can concatenate the strings as follows: "<span class="tex-font-style-tt">(</span>"&nbsp;$+$&nbsp;"<span class="tex-font-style-tt">)</span>"&nbsp;$+$&nbsp;"<span class="tex-font-style-tt">()()())</span>"&nbsp;$+$&nbsp;"<span class="tex-font-style-tt">(</span>"&nbsp;$=$&nbsp;"<span class="tex-font-style-tt">()()()())(</span>", the resulting string will have four prefixes that are RBS: "<span class="tex-font-style-tt">()</span>", "<span class="tex-font-style-tt">()()</span>", "<span class="tex-font-style-tt">()()()</span>", "<span class="tex-font-style-tt">()()()()</span>".</p><p>The third and the fourth examples contain only one string each, so the order is fixed.</p>
