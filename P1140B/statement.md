## Description

<div><p>You have a string $s$ of length $n$ consisting of only characters <span class="tex-font-style-tt">&gt;</span> and <span class="tex-font-style-tt">&lt;</span>. You may do some operations with this string, for each operation you have to choose some character that still remains in the string. If you choose a character <span class="tex-font-style-tt">&gt;</span>, the character that comes right after it is deleted (if the character you chose was the last one, nothing happens). If you choose a character <span class="tex-font-style-tt">&lt;</span>, the character that comes right before it is deleted (if the character you chose was the first one, nothing happens).</p><p>For example, if we choose character <span class="tex-font-style-tt">&gt;</span> in string <span class="tex-font-style-tt">&gt; <span class="tex-font-style-bf">&gt;</span> &lt; &gt;</span>, the string will become to <span class="tex-font-style-tt">&gt; &gt; &gt;</span>. And if we choose character <span class="tex-font-style-tt">&lt;</span> in string <span class="tex-font-style-tt">&gt; <span class="tex-font-style-bf">&lt;</span></span>, the string will become to <span class="tex-font-style-tt">&lt;</span>.</p><p>The string is good if there is a sequence of operations such that after performing it only one character will remain in the string. For example, the strings <span class="tex-font-style-tt">&gt;</span>, <span class="tex-font-style-tt">&gt; &gt;</span> are good. </p><p><span class="tex-font-style-bf">Before applying the operations</span>, you may remove any number of characters from the given string (possibly none, possibly up to $n - 1$, but not the whole string). You need to calculate the minimum number of characters to be deleted from string $s$ so that it becomes good.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) – the number of test cases. Each test case is represented by two lines.</p><p>The first line of $i$-th test case contains one integer $n$ ($1 \le n \le 100$) – the length of string $s$.</p><p>The second line of $i$-th test case contains string $s$, consisting of only characters <span class="tex-font-style-tt">&gt;</span> and <span class="tex-font-style-tt">&lt;</span>.</p></div><div class="output-specification"><p>For each test case print one line.</p><p>For $i$-th test case print the minimum number of characters to be deleted from string $s$ so that it becomes good.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) – the number of test cases. Each test case is represented by two lines.</p><p>The first line of $i$-th test case contains one integer $n$ ($1 \le n \le 100$) – the length of string $s$.</p><p>The second line of $i$-th test case contains string $s$, consisting of only characters <span class="tex-font-style-tt">&gt;</span> and <span class="tex-font-style-tt">&lt;</span>.</p>

## Output

<p>For each test case print one line.</p><p>For $i$-th test case print the minimum number of characters to be deleted from string $s$ so that it becomes good.</p>





```input1
3
2
&lt;&gt;
3
&gt;&lt;&lt;
1
&gt;
```




```output1
1
0
0
```



## Note

<p>In the first test case we can delete any character in string <span class="tex-font-style-tt">&lt;&gt;</span>.</p><p>In the second test case we don't need to delete any characters. The string <span class="tex-font-style-tt">&gt; &lt; &lt;</span> is good, because we can perform the following sequence of operations: <span class="tex-font-style-tt">&gt; <span class="tex-font-style-bf">&lt;</span> &lt;</span> $\rightarrow$ <span class="tex-font-style-tt">&lt; <span class="tex-font-style-bf">&lt;</span></span> $\rightarrow$ <span class="tex-font-style-tt">&lt;</span>.</p>
