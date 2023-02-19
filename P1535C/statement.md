## Description

<div><p>You are given a string $s$ consisting of the characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>.</p><p>Let's call a string <span class="tex-font-style-bf">unstable</span> if it consists of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span> and any two adjacent characters are different (i.&nbsp;e. it has the form <span class="tex-font-style-tt">010101...</span> or <span class="tex-font-style-tt">101010...</span>).</p><p>Let's call a string <span class="tex-font-style-bf">beautiful</span> if it consists of the characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>, and you can replace the characters <span class="tex-font-style-tt">?</span> to <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span> (for each character, the choice is independent), so that the string becomes <span class="tex-font-style-bf">unstable</span>.</p><p>For example, the strings <span class="tex-font-style-tt">0??10</span>, <span class="tex-font-style-tt">0</span>, and <span class="tex-font-style-tt">???</span> are beautiful, and the strings <span class="tex-font-style-tt">00</span> and <span class="tex-font-style-tt">?1??1</span> are not.</p><p>Calculate the number of beautiful contiguous substrings of the string $s$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— number of test cases.</p><p>The first and only line of each test case contains the string $s$ ($1 \le |s| \le 2 \cdot 10^5$) consisting of characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>.</p><p>It is guaranteed that the sum of the string lengths over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the number of <span class="tex-font-style-bf">beautiful</span> substrings of the string $s$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— number of test cases.</p><p>The first and only line of each test case contains the string $s$ ($1 \le |s| \le 2 \cdot 10^5$) consisting of characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>.</p><p>It is guaranteed that the sum of the string lengths over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the number of <span class="tex-font-style-bf">beautiful</span> substrings of the string $s$.</p>





```input1
3
0?10
???
?10??1100
```




```output1
8
6
25
```


