## Description

<div><p>You are given a string $s$, consisting of brackets of two types: '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>', '<span class="tex-font-style-tt">[</span>' and '<span class="tex-font-style-tt">]</span>'.</p><p>A string is called a regular bracket sequence (RBS) if it's of one of the following types: </p><ul> <li> empty string; </li><li> '<span class="tex-font-style-tt">(</span>' + RBS + '<span class="tex-font-style-tt">)</span>'; </li><li> '<span class="tex-font-style-tt">[</span>' + RBS + '<span class="tex-font-style-tt">]</span>'; </li><li> RBS + RBS. </li></ul><p>where plus is a concatenation of two strings.</p><p>In one move you can choose a non-empty subsequence of the string $s$ (not necessarily consecutive) that is an RBS, remove it from the string and concatenate the remaining parts without changing the order.</p><p>What is the maximum number of moves you can perform?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Each of the next $t$ lines contains a non-empty string, consisting only of characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>', '<span class="tex-font-style-tt">[</span>' and '<span class="tex-font-style-tt">]</span>'. The total length of the strings over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase print a single integer&nbsp;— the maximum number of moves you can perform on a given string $s$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Each of the next $t$ lines contains a non-empty string, consisting only of characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>', '<span class="tex-font-style-tt">[</span>' and '<span class="tex-font-style-tt">]</span>'. The total length of the strings over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase print a single integer&nbsp;— the maximum number of moves you can perform on a given string $s$.</p>





```input1
5
()
[]()
([)]
)]([
)[(]
```




```output1
1
2
2
0
1
```



## Note

<p>In the first example you can just erase the whole string.</p><p>In the second example you can first erase the brackets on positions $1$ and $2$: "<span class="tex-font-style-tt"><span class="tex-font-style-bf">[]</span>()</span>", then "<span class="tex-font-style-tt">()</span>" is left. After that you can erase it whole. You could erase the whole string from the beginning but you would get one move instead of two.</p><p>In the third example you can first erase the brackets on positions $1$ and $3$: "<span class="tex-font-style-tt"><span class="tex-font-style-bf">(</span>[<span class="tex-font-style-bf">)</span>]</span>". They form an RBS "<span class="tex-font-style-tt">()</span>". Then "<span class="tex-font-style-tt">[]</span>" is left, so you can erase it whole.</p><p>In the fourth example there is no subsequence that is an RBS, so you can't perform a move at all.</p><p>In the fifth example you can erase the brackets on positions $2$ and $4$: "<span class="tex-font-style-tt">)<span class="tex-font-style-bf">[</span>(<span class="tex-font-style-bf">]</span></span>" and get "<span class="tex-font-style-tt">)(</span>" as a result. You can erase nothing from it.</p>
