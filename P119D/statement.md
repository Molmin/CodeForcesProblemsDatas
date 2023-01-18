## Description

<div><p>Let <span class="tex-span"><i>s</i></span> be a string whose length equals <span class="tex-span"><i>n</i></span>. Its characters are numbered from 0 to <span class="tex-span"><i>n</i> - 1</span>, <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are integers, <span class="tex-span">0 ≤ <i>i</i> &lt; <i>j</i> &lt; <i>n</i></span>. Let's define function <span class="tex-span"><i>f</i></span> as follows:</p><p><span class="tex-span"><i>f</i>(<i>s</i>, <i>i</i>, <i>j</i>) = <i>s</i>[<i>i</i> + 1... <i>j</i> - 1] + <i>r</i>(<i>s</i>[<i>j</i>... <i>n</i> - 1]) + <i>r</i>(<i>s</i>[0... <i>i</i>])</span>.</p><p>Here <span class="tex-span"><i>s</i>[<i>p</i>... <i>q</i>]</span> is a substring of string <span class="tex-span"><i>s</i></span>, that starts in position <span class="tex-span"><i>p</i></span> and ends in position <span class="tex-span"><i>q</i></span> (inclusive); "<span class="tex-font-style-tt">+</span>" is the string concatenation operator; <span class="tex-span"><i>r</i>(<i>x</i>)</span> is a string resulting from writing the characters of the <span class="tex-span"><i>x</i></span> string in the reverse order. If <span class="tex-span"><i>j</i> = <i>i</i> + 1</span>, then the substring <span class="tex-span"><i>s</i>[<i>i</i> + 1... <i>j</i> - 1]</span> is considered empty.</p><p>You are given two strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Find such values of <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, that <span class="tex-span"><i>f</i>(<i>a</i>, <i>i</i>, <i>j</i>) = <i>b</i></span>. Number <span class="tex-span"><i>i</i></span> should be maximally possible. If for this <span class="tex-span"><i>i</i></span> there exists several valid values of <span class="tex-span"><i>j</i></span>, choose the minimal <span class="tex-span"><i>j</i></span>.</p></div><div class="input-specification"><p>The first two input lines are non-empty strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> correspondingly. Each string's length does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. The strings can contain any characters with ASCII codes from 32 to 126 inclusive.</p></div><div class="output-specification"><p>Print two integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> — the answer to the problem. If no solution exists, print "<span class="tex-font-style-tt">-1 -1</span>" (without the quotes).</p></div>

## Input

<p>The first two input lines are non-empty strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> correspondingly. Each string's length does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. The strings can contain any characters with ASCII codes from 32 to 126 inclusive.</p>

## Output

<p>Print two integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> — the answer to the problem. If no solution exists, print "<span class="tex-font-style-tt">-1 -1</span>" (without the quotes).</p>





```input1
Die Polizei untersucht eine Straftat im IT-Bereich.
untersucht eine Straftat.hciereB-TI mi  ieziloP eiD

```




```input2
cbaaaa
aaaabc

```




```input3
123342
3324212

```




```output1
11 36

```




```output2
4 5

```




```output3
-1 -1
```


