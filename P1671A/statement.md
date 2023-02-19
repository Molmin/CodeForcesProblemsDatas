## Description

<div><p>You are given a string $s$. You have to determine whether it is possible to build the string $s$ out of strings <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">aaa</span>, <span class="tex-font-style-tt">bb</span> and/or <span class="tex-font-style-tt">bbb</span> by concatenating them. You can use the strings <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">aaa</span>, <span class="tex-font-style-tt">bb</span> and/or <span class="tex-font-style-tt">bbb</span> any number of times and in any order.</p><p>For example:</p><ul> <li> <span class="tex-font-style-tt">aaaabbb</span> can be built as <span class="tex-font-style-tt">aa</span> $+$ <span class="tex-font-style-tt">aa</span> $+$ <span class="tex-font-style-tt">bbb</span>; </li><li> <span class="tex-font-style-tt">bbaaaaabbb</span> can be built as <span class="tex-font-style-tt">bb</span> $+$ <span class="tex-font-style-tt">aaa</span> $+$ <span class="tex-font-style-tt">aa</span> $+$ <span class="tex-font-style-tt">bbb</span>; </li><li> <span class="tex-font-style-tt">aaaaaa</span> can be built as <span class="tex-font-style-tt">aa</span> $+$ <span class="tex-font-style-tt">aa</span> $+$ <span class="tex-font-style-tt">aa</span>; </li><li> <span class="tex-font-style-tt">abab</span> cannot be built from <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">aaa</span>, <span class="tex-font-style-tt">bb</span> and/or <span class="tex-font-style-tt">bbb</span>. </li></ul></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of one line containing the string $s$ ($1 \le |s| \le 50$), consisting of characters <span class="tex-font-style-tt">a</span> and/or <span class="tex-font-style-tt">b</span>.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to build the string $s$. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of one line containing the string $s$ ($1 \le |s| \le 50$), consisting of characters <span class="tex-font-style-tt">a</span> and/or <span class="tex-font-style-tt">b</span>.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to build the string $s$. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p>





```input1
8
aaaabbb
bbaaaaabbb
aaaaaa
abab
a
b
aaaab
bbaaa
```




```output1
YES
YES
YES
NO
NO
NO
NO
YES
```



## Note

<p>The first four test cases of the example are described in the statement.</p>
