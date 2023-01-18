## Description

<div><p>A string is called beautiful if no two consecutive characters are equal. For example, "<span class="tex-font-style-tt">ababcb</span>", "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">abab</span>" are beautiful strings, while "<span class="tex-font-style-tt">aaaaaa</span>", "<span class="tex-font-style-tt">abaa</span>" and "<span class="tex-font-style-tt">bb</span>" are not.</p><p>Ahcl wants to construct a beautiful string. He has a string $s$, consisting of only characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>' and '<span class="tex-font-style-tt">?</span>'. Ahcl needs to replace each character '<span class="tex-font-style-tt">?</span>' with one of the three characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' or '<span class="tex-font-style-tt">c</span>', such that the resulting string is beautiful. Please help him!</p><p>More formally, after replacing all characters '<span class="tex-font-style-tt">?</span>', the condition $s_i \neq s_{i+1}$ should be satisfied for all $1 \leq i \leq |s| - 1$, where $|s|$ is the length of the string $s$.</p></div><div class="input-specification"><p>The first line contains positive integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. Next $t$ lines contain the descriptions of test cases.</p><p>Each line contains a non-empty string $s$ consisting of only characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>' and '<span class="tex-font-style-tt">?</span>'. </p><p>It is guaranteed that in each test case a string $s$ has at least one character '<span class="tex-font-style-tt">?</span>'. The sum of lengths of strings $s$ in all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case given in the input print the answer in the following format:</p><ul> <li> If it is impossible to create a beautiful string, print "<span class="tex-font-style-tt">-1</span>" (without quotes); </li><li> Otherwise, print the resulting beautiful string after replacing all '<span class="tex-font-style-tt">?</span>' characters. If there are multiple answers, you can print any of them. </li></ul></div>

## Input

<p>The first line contains positive integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. Next $t$ lines contain the descriptions of test cases.</p><p>Each line contains a non-empty string $s$ consisting of only characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>' and '<span class="tex-font-style-tt">?</span>'. </p><p>It is guaranteed that in each test case a string $s$ has at least one character '<span class="tex-font-style-tt">?</span>'. The sum of lengths of strings $s$ in all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case given in the input print the answer in the following format:</p><ul> <li> If it is impossible to create a beautiful string, print "<span class="tex-font-style-tt">-1</span>" (without quotes); </li><li> Otherwise, print the resulting beautiful string after replacing all '<span class="tex-font-style-tt">?</span>' characters. If there are multiple answers, you can print any of them. </li></ul>





```input1
3
a???cb
a??bbc
a?b?c
```




```output1
ababcb
-1
acbac
```



## Note

<p>In the first test case, all possible correct answers are "<span class="tex-font-style-tt">ababcb</span>", "<span class="tex-font-style-tt">abcacb</span>", "<span class="tex-font-style-tt">abcbcb</span>", "<span class="tex-font-style-tt">acabcb</span>" and "<span class="tex-font-style-tt">acbacb</span>". The two answers "<span class="tex-font-style-tt">abcbab</span>" and "<span class="tex-font-style-tt">abaabc</span>" are incorrect, because you can replace only '<span class="tex-font-style-tt">?</span>' characters and the resulting string must be beautiful.</p><p>In the second test case, it is impossible to create a beautiful string, because the $4$-th and $5$-th characters will be always equal.</p><p>In the third test case, the only answer is "<span class="tex-font-style-tt">acbac</span>".</p>
