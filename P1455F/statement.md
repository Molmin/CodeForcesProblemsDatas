## Description

<div><p>You are given a string $s$ consisting of $n$ characters. These characters are among the first $k$ lowercase letters of the Latin alphabet. You have to perform $n$ operations with the string.</p><p>During the $i$-th operation, you take the character that <span class="tex-font-style-bf">initially occupied</span> the $i$-th position, and perform <span class="tex-font-style-bf">one</span> of the following actions with it:</p><ul> <li> swap it with the previous character in the string (if it exists). This operation is represented as <span class="tex-font-style-tt">L</span>; </li><li> swap it with the next character in the string (if it exists). This operation is represented as <span class="tex-font-style-tt">R</span>; </li><li> cyclically change it to the previous character in the alphabet (<span class="tex-font-style-tt">b</span> becomes <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">c</span> becomes <span class="tex-font-style-tt">b</span>, and so on; <span class="tex-font-style-tt">a</span> becomes the $k$-th letter of the Latin alphabet). This operation is represented as <span class="tex-font-style-tt">D</span>; </li><li> cyclically change it to the next character in the alphabet (<span class="tex-font-style-tt">a</span> becomes <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">b</span> becomes <span class="tex-font-style-tt">c</span>, and so on; the $k$-th letter of the Latin alphabet becomes <span class="tex-font-style-tt">a</span>). This operation is represented as <span class="tex-font-style-tt">U</span>; </li><li> do nothing. This operation is represented as <span class="tex-font-style-tt">0</span>. </li></ul><p>For example, suppose the initial string is <span class="tex-font-style-tt">test</span>, $k = 20$, and the sequence of operations is <span class="tex-font-style-tt">URLD</span>. Then the string is transformed as follows:</p><ol> <li> the first operation is <span class="tex-font-style-tt">U</span>, so we change the underlined letter in <span class="tex-font-style-tt"><span class="tex-font-style-underline">t</span>est</span> to the next one in the first $20$ Latin letters, which is <span class="tex-font-style-tt">a</span>. The string is now <span class="tex-font-style-tt">aest</span>; </li><li> the second operation is <span class="tex-font-style-tt">R</span>, so we swap the underlined letter with the next one in the string <span class="tex-font-style-tt">a<span class="tex-font-style-underline">e</span>st</span>. The string is now <span class="tex-font-style-tt">aset</span>; </li><li> the third operation is <span class="tex-font-style-tt">L</span>, so we swap the underlined letter with the previous one in the string <span class="tex-font-style-tt">a<span class="tex-font-style-underline">s</span>et</span> (note that this is now the $2$-nd character of the string, but it was initially the $3$-rd one, so the $3$-rd operation is performed to it). The resulting string is <span class="tex-font-style-tt">saet</span>; </li><li> the fourth operation is <span class="tex-font-style-tt">D</span>, so we change the underlined letter in <span class="tex-font-style-tt">sae<span class="tex-font-style-underline">t</span></span> to the previous one in the first $20$ Latin letters, which is <span class="tex-font-style-tt">s</span>. The string is now <span class="tex-font-style-tt">saes</span>. </li></ol><p>The result of performing the sequence of operations is <span class="tex-font-style-tt">saes</span>.</p><p>Given the string $s$ and the value of $k$, find the lexicographically smallest string that can be obtained after applying a sequence of operations to $s$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains two integers $n$ and $k$ ($1 \le n \le 500$; $2 \le k \le 26$). </p><p>The second line contains a string $s$ consisting of $n$ characters. Each character is one of the $k$ first letters of the Latin alphabet (in lower case).</p></div><div class="output-specification"><p>For each test case, print one line containing the lexicographically smallest string that can be obtained from $s$ using one sequence of operations.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains two integers $n$ and $k$ ($1 \le n \le 500$; $2 \le k \le 26$). </p><p>The second line contains a string $s$ consisting of $n$ characters. Each character is one of the $k$ first letters of the Latin alphabet (in lower case).</p>

## Output

<p>For each test case, print one line containing the lexicographically smallest string that can be obtained from $s$ using one sequence of operations.</p>





```input1
6
4 2
bbab
7 5
cceddda
6 5
ecdaed
7 4
dcdbdaa
8 3
ccabbaca
5 7
eabba
```




```output1
aaaa
baccacd
aabdac
aabacad
aaaaaaaa
abadb
```


