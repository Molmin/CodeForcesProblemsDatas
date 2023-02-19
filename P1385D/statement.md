## Description

<div><p>You are given a string $s[1 \dots n]$ consisting of lowercase Latin letters. It is guaranteed that $n = 2^k$ for some integer $k \ge 0$.</p><p>The string $s[1 \dots n]$ is called <span class="tex-font-style-it">$c$-good</span> if <span class="tex-font-style-bf">at least one</span> of the following three conditions is satisfied:</p><ul> <li> The length of $s$ is $1$, and it consists of the character $c$ (i.e. $s_1=c$);</li><li> The length of $s$ is greater than $1$, the first half of the string consists of only the character $c$ (i.e. $s_1=s_2=\dots=s_{\frac{n}{2}}=c$) and the second half of the string (i.e. the string $s_{\frac{n}{2} + 1}s_{\frac{n}{2} + 2} \dots s_n$) is a <span class="tex-font-style-it">$(c+1)$-good</span> string; </li><li> The length of $s$ is greater than $1$, the second half of the string consists of only the character $c$ (i.e. $s_{\frac{n}{2} + 1}=s_{\frac{n}{2} + 2}=\dots=s_n=c$) and the first half of the string (i.e. the string $s_1s_2 \dots s_{\frac{n}{2}}$) is a <span class="tex-font-style-it">$(c+1)$-good</span> string. </li></ul><p>For example: "<span class="tex-font-style-tt">aabc</span>" is <span class="tex-font-style-it">'<span class="tex-font-style-tt">a</span>'-good</span>, "<span class="tex-font-style-tt">ffgheeee</span>" is <span class="tex-font-style-it">'<span class="tex-font-style-tt">e</span>'-good</span>.</p><p>In one move, you can choose one index $i$ from $1$ to $n$ and replace $s_i$ with any lowercase Latin letter (any character from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>').</p><p>Your task is to find the minimum number of moves required to obtain an <span class="tex-font-style-it">'<span class="tex-font-style-tt">a</span>'-good</span> string from $s$ (i.e. <span class="tex-font-style-it">$c$-good string</span> for $c=$ '<span class="tex-font-style-tt">a</span>'). It is guaranteed that the answer always exists.</p><p>You have to answer $t$ independent test cases.</p><p>Another example of an <span class="tex-font-style-it">'<span class="tex-font-style-tt">a</span>'-good</span> string is as follows. Consider the string $s = $"<span class="tex-font-style-tt">cdbbaaaa</span>". It is an <span class="tex-font-style-it">'<span class="tex-font-style-tt">a</span>'-good</span> string, because:</p><ul> <li> the second half of the string ("<span class="tex-font-style-tt">aaaa</span>") consists of only the character '<span class="tex-font-style-tt">a</span>'; </li><li> the first half of the string ("<span class="tex-font-style-tt">cdbb</span>") is <span class="tex-font-style-it">'<span class="tex-font-style-tt">b</span>'-good</span> string, because: <ul> <li> the second half of the string ("<span class="tex-font-style-tt">bb</span>") consists of only the character '<span class="tex-font-style-tt">b</span>'; </li><li> the first half of the string ("<span class="tex-font-style-tt">cd</span>") is <span class="tex-font-style-it">'<span class="tex-font-style-tt">c</span>'-good</span> string, because: <ul> <li> the first half of the string ("<span class="tex-font-style-tt">c</span>") consists of only the character '<span class="tex-font-style-tt">c</span>'; </li><li> the second half of the string ("<span class="tex-font-style-tt">d</span>") is <span class="tex-font-style-it">'<span class="tex-font-style-tt">d</span>'-good</span> string. </li></ul> </li></ul> </li></ul></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 131~072$) — the length of $s$. It is guaranteed that $n = 2^k$ for some integer $k \ge 0$. The second line of the test case contains the string $s$ consisting of $n$ lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer — the minimum number of moves required to obtain an <span class="tex-font-style-it">'<span class="tex-font-style-tt">a</span>'-good</span> string from $s$ (i.e. <span class="tex-font-style-it">$c$-good string</span> with $c =$ '<span class="tex-font-style-tt">a</span>'). It is guaranteed that the answer exists.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 131~072$) — the length of $s$. It is guaranteed that $n = 2^k$ for some integer $k \ge 0$. The second line of the test case contains the string $s$ consisting of $n$ lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer — the minimum number of moves required to obtain an <span class="tex-font-style-it">'<span class="tex-font-style-tt">a</span>'-good</span> string from $s$ (i.e. <span class="tex-font-style-it">$c$-good string</span> with $c =$ '<span class="tex-font-style-tt">a</span>'). It is guaranteed that the answer exists.</p>





```input1
6
8
bbdcaaaa
8
asdfghjk
8
ceaaaabb
8
bbaaddcc
1
z
2
ac
```




```output1
0
7
4
5
1
1
```


