## Description

<div><p><span class="tex-font-style-it">This is the easy version of this problem. The only difference is the limit of $n$ - the length of the input string. In this version, $1 \leq n \leq 2000$. The hard version of this challenge is not offered in the round for the second division. </span></p><p>Let's define a correct bracket sequence and its depth as follow:</p><ul> <li> An empty string is a correct bracket sequence with depth $0$. </li><li> If "<span class="tex-font-style-tt">s</span>" is a correct bracket sequence with depth $d$ then "<span class="tex-font-style-tt">(s)</span>" is a correct bracket sequence with depth $d + 1$. </li><li> If "<span class="tex-font-style-tt">s</span>" and "<span class="tex-font-style-tt">t</span>" are both correct bracket sequences then their concatenation "<span class="tex-font-style-tt">st</span>" is a correct bracket sequence with depth equal to the maximum depth of $s$ and $t$. </li></ul><p>For a (not necessarily correct) bracket sequence $s$, we define its depth as the maximum depth of any <span class="tex-font-style-bf">correct</span> bracket sequence induced by removing some characters from $s$ (possibly zero). For example: the bracket sequence $s = $"<span class="tex-font-style-tt">())(())</span>" has depth $2$, because by removing the third character we obtain a correct bracket sequence "<span class="tex-font-style-tt">()(())</span>" with depth $2$.</p><p>Given a string $a$ consists of only characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' and '<span class="tex-font-style-tt">?</span>'. Consider all (not necessarily correct) bracket sequences obtained by replacing all characters '<span class="tex-font-style-tt">?</span>' in $a$ by either '<span class="tex-font-style-tt">(</span>' or '<span class="tex-font-style-tt">)</span>'. Calculate the sum of all the depths of all these bracket sequences. As this number can be large, find it modulo $998244353$.</p><p><span class="tex-font-style-bf">Hacks</span> in this problem in the first division can be done only if easy and hard versions of this problem was solved.</p></div><div class="input-specification"><p>The only line contains a non-empty string consist of only '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' and '<span class="tex-font-style-tt">?</span>'. The length of the string is at most $2000$.</p></div><div class="output-specification"><p>Print the answer modulo $998244353$ in a single line.</p></div>

## Input

<p>The only line contains a non-empty string consist of only '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' and '<span class="tex-font-style-tt">?</span>'. The length of the string is at most $2000$.</p>

## Output

<p>Print the answer modulo $998244353$ in a single line.</p>





```input1
??
```




```input2
(?(?))
```




```output1
1
```




```output2
9
```



## Note

<p>In the first test case, we can obtain $4$ bracket sequences by replacing all characters '<span class="tex-font-style-tt">?</span>' with either '<span class="tex-font-style-tt">(</span>' or '<span class="tex-font-style-tt">)</span>':</p><ul> <li> "<span class="tex-font-style-tt">((</span>". Its depth is $0$; </li><li> "<span class="tex-font-style-tt">))</span>". Its depth is $0$; </li><li> "<span class="tex-font-style-tt">)(</span>". Its depth is $0$; </li><li> "<span class="tex-font-style-tt">()</span>". Its depth is $1$. </li></ul><p>So, the answer is $1 = 0 + 0 + 0 + 1$.</p><p>In the second test case, we can obtain $4$ bracket sequences by replacing all characters '<span class="tex-font-style-tt">?</span>' with either '<span class="tex-font-style-tt">(</span>' or '<span class="tex-font-style-tt">)</span>':</p><ul> <li> "<span class="tex-font-style-tt">(((())</span>". Its depth is $2$; </li><li> "<span class="tex-font-style-tt">()()))</span>". Its depth is $2$; </li><li> "<span class="tex-font-style-tt">((()))</span>". Its depth is $3$; </li><li> "<span class="tex-font-style-tt">()(())</span>". Its depth is $2$. </li></ul><p>So, the answer is $9 = 2 + 2 + 3 + 2$.</p>
