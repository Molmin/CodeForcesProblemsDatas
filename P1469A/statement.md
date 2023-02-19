## Description

<div><p>A bracket sequence is called regular if it is possible to obtain correct arithmetic expression by inserting characters <span class="tex-font-style-tt">+</span> and <span class="tex-font-style-tt">1</span> into this sequence. For example, sequences <span class="tex-font-style-tt">(())()</span>, <span class="tex-font-style-tt">()</span> and <span class="tex-font-style-tt">(()(()))</span> are regular, while <span class="tex-font-style-tt">)(</span>, <span class="tex-font-style-tt">(()</span> and <span class="tex-font-style-tt">(()))(</span> are not. Let's call a regular bracket sequence "RBS".</p><p>You are given a sequence $s$ of $n$ characters <span class="tex-font-style-tt">(</span>, <span class="tex-font-style-tt">)</span>, and/or <span class="tex-font-style-tt">?</span>. <span class="tex-font-style-bf">There is exactly one character <span class="tex-font-style-tt">(</span> and exactly one character <span class="tex-font-style-tt">)</span></span> in this sequence.</p><p>You have to replace every character <span class="tex-font-style-tt">?</span> with either <span class="tex-font-style-tt">)</span> or <span class="tex-font-style-tt">(</span> (different characters <span class="tex-font-style-tt">?</span> can be replaced with different brackets). <span class="tex-font-style-bf">You cannot reorder the characters, remove them, insert other characters, and each <span class="tex-font-style-tt">?</span> must be replaced</span>.</p><p>Determine if it is possible to obtain an RBS after these replacements.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of one line containing $s$ ($2 \le |s| \le 100$) — a sequence of characters <span class="tex-font-style-tt">(</span>, <span class="tex-font-style-tt">)</span>, and/or <span class="tex-font-style-tt">?</span>. <span class="tex-font-style-bf">There is exactly one character <span class="tex-font-style-tt">(</span> and exactly one character <span class="tex-font-style-tt">)</span></span> in this sequence.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to obtain a regular bracket sequence, or <span class="tex-font-style-tt">NO</span> otherwise}. </p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of one line containing $s$ ($2 \le |s| \le 100$) — a sequence of characters <span class="tex-font-style-tt">(</span>, <span class="tex-font-style-tt">)</span>, and/or <span class="tex-font-style-tt">?</span>. <span class="tex-font-style-bf">There is exactly one character <span class="tex-font-style-tt">(</span> and exactly one character <span class="tex-font-style-tt">)</span></span> in this sequence.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to obtain a regular bracket sequence, or <span class="tex-font-style-tt">NO</span> otherwise}. </p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer).</p>





```input1
5
()
(?)
(??)
??()
)?(?
```




```output1
YES
NO
YES
YES
NO
```



## Note

<p>In the first test case, the sequence is already an RBS.</p><p>In the third test case, you can obtain an RBS as follows: <span class="tex-font-style-tt">()()</span> or <span class="tex-font-style-tt">(())</span>.</p><p>In the fourth test case, you can obtain an RBS as follows: <span class="tex-font-style-tt">()()</span>.</p>
