## Description

<div><p>You are given a number $k$ and a string $s$ of length $n$, consisting of the characters '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">*</span>'. You want to replace some of the '<span class="tex-font-style-tt">*</span>' characters with '<span class="tex-font-style-tt">x</span>' characters so that the following conditions are met: </p><ul> <li> The first character '<span class="tex-font-style-tt">*</span>' in the original string should be replaced with '<span class="tex-font-style-tt">x</span>'; </li><li> The last character '<span class="tex-font-style-tt">*</span>' in the original string should be replaced with '<span class="tex-font-style-tt">x</span>'; </li><li> The distance between two neighboring replaced characters '<span class="tex-font-style-tt">x</span>' must not exceed $k$ (more formally, if you replaced characters at positions $i$ and $j$ ($i &lt; j$) and at positions $[i+1, j-1]$ there is no <span class="tex-font-style-tt">"x"</span> symbol, then $j-i$ must be no more than $k$). </li></ul><p>For example, if $n=7$, $s=$<span class="tex-font-style-tt">.**.***</span> and $k=3$, then the following strings will satisfy the conditions above: </p><ul> <li> <span class="tex-font-style-tt">.xx.*xx</span>; </li><li> <span class="tex-font-style-tt">.x*.x*x</span>; </li><li> <span class="tex-font-style-tt">.xx.xxx</span>. </li></ul> But, for example, the following strings will not meet the conditions: <ul> <li> <span class="tex-font-style-tt">.**.*xx</span> (the first character '<span class="tex-font-style-tt">*</span>' should be replaced with '<span class="tex-font-style-tt">x</span>'); </li><li> <span class="tex-font-style-tt">.x*.xx*</span> (the last character '<span class="tex-font-style-tt">*</span>' should be replaced with '<span class="tex-font-style-tt">x</span>'); </li><li> <span class="tex-font-style-tt">.x*.*xx</span> (the distance between characters at positions $2$ and $6$ is greater than $k=3$). </li></ul><p>Given $n$, $k$, and $s$, find the minimum number of '<span class="tex-font-style-tt">*</span>' characters that must be replaced with '<span class="tex-font-style-tt">x</span>' in order to meet the above conditions.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 500$). Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 50$).</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of the characters '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">*</span>'.</p><p>It is guaranteed that there is at least one '<span class="tex-font-style-tt">*</span>' in the string $s$.</p><p>It is guaranteed that the distance between any two neighboring '<span class="tex-font-style-tt">*</span>' characters does not exceed $k$.</p></div><div class="output-specification"><p>For each test case output the minimum number of '<span class="tex-font-style-tt">*</span>' characters that must be replaced with '<span class="tex-font-style-tt">x</span>' characters in order to satisfy the conditions above.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 500$). Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 50$).</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of the characters '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">*</span>'.</p><p>It is guaranteed that there is at least one '<span class="tex-font-style-tt">*</span>' in the string $s$.</p><p>It is guaranteed that the distance between any two neighboring '<span class="tex-font-style-tt">*</span>' characters does not exceed $k$.</p>

## Output

<p>For each test case output the minimum number of '<span class="tex-font-style-tt">*</span>' characters that must be replaced with '<span class="tex-font-style-tt">x</span>' characters in order to satisfy the conditions above.</p>





```input1
5
7 3
.**.***
5 1
..*..
5 2
*.*.*
3 2
*.*
1 1
*
```




```output1
3
1
3
2
1
```


