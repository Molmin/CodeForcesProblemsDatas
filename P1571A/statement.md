## Description

<div><p>Once upon a time, Petya had an array of integers $a$ of length $n$. But over time, the array itself was lost, and only $n-1$ results of comparisons of neighboring array elements remained. In other words, for every $i$ from $1$ to $n-1$, Petya knows exactly one of these three facts:</p><ul> <li> $a_i &lt; a_{i+1}$; </li><li> $a_i = a_{i+1}$; </li><li> $a_i &gt; a_{i+1}$. </li></ul><p>Petya wonders if it is possible to uniquely determine the result of comparing $a_1$ and $a_n$.</p><p>You have to help Petya determine the result of comparing $a_1$ and $a_n$ or report that the result cannot be determined unambiguously.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases.</p><p>The only line of the test case contains the string $s$ ($1 \le |s| \le 100$), where $s_i$ is:</p><ul> <li> <span class="tex-font-style-tt">&lt;</span>, if $a_i &lt; a_{i + 1}$; </li><li> <span class="tex-font-style-tt">&gt;</span>, if $a_i &gt; a_{i + 1}$; </li><li> <span class="tex-font-style-tt">=</span>, if $a_i = a_{i + 1}$. </li></ul></div><div class="output-specification"><p>For each test case, print a single string equal to:</p><ul> <li> <span class="tex-font-style-tt">&lt;</span>, if $a_1 &lt; a_n$; </li><li> <span class="tex-font-style-tt">&gt;</span>, if $a_1 &gt; a_n$; </li><li> <span class="tex-font-style-tt">=</span>, if $a_1 = a_n$; </li><li> <span class="tex-font-style-tt">?</span>, if it is impossible to uniquely determine the result of the comparison. </li></ul></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases.</p><p>The only line of the test case contains the string $s$ ($1 \le |s| \le 100$), where $s_i$ is:</p><ul> <li> <span class="tex-font-style-tt">&lt;</span>, if $a_i &lt; a_{i + 1}$; </li><li> <span class="tex-font-style-tt">&gt;</span>, if $a_i &gt; a_{i + 1}$; </li><li> <span class="tex-font-style-tt">=</span>, if $a_i = a_{i + 1}$. </li></ul>

## Output

<p>For each test case, print a single string equal to:</p><ul> <li> <span class="tex-font-style-tt">&lt;</span>, if $a_1 &lt; a_n$; </li><li> <span class="tex-font-style-tt">&gt;</span>, if $a_1 &gt; a_n$; </li><li> <span class="tex-font-style-tt">=</span>, if $a_1 = a_n$; </li><li> <span class="tex-font-style-tt">?</span>, if it is impossible to uniquely determine the result of the comparison. </li></ul>





```input1
4
&gt;&gt;&gt;
&lt;&gt;&lt;=&lt;
=
&lt;&lt;==
```




```output1
&gt;
?
=
&lt;
```



## Note

<p>Consider the test cases of the example:</p><ul> <li> in the first test case, it's easy to see that $a_1 &gt; a_4$ since $a_1 &gt; a_2 &gt; a_3 &gt; a_4$; </li><li> in the second test case, both sequences $[1, 2, 0, 10, 10, 15]$ and $[10, 11, 1, 2, 2, 5]$ meet the constraints; in the first one, $a_1 &lt; a_6$, and in the second one, $a_1 &gt; a_6$, so it's impossible to compare $a_1$ and $a_6$; </li><li> in the third test case, we already know that $a_1 = a_2$; </li><li> in the fourth test case, it's easy to see that $a_3 = a_4 = a_5$, and $a_1 &lt; a_2 &lt; a_3$, so $a_1 &lt; a_5$. </li></ul>
