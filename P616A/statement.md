## Description

<div><p>You are given two very long integers <span class="tex-span"><i>a</i>, <i>b</i></span> (leading zeroes are allowed). You should check what number <span class="tex-span"><i>a</i></span> or <span class="tex-span"><i>b</i></span> is greater or determine that they are equal.</p><p>The input size is very large so don't use the reading of symbols one by one. Instead of that use the reading of a whole line or token.</p><p>As input/output can reach huge size it is recommended to use fast input/output methods: for example, prefer to use <span class="tex-font-style-tt">scanf/printf</span> instead of <span class="tex-font-style-tt">cin/cout</span> in C++, prefer to use <span class="tex-font-style-tt">BufferedReader/PrintWriter</span> instead of <span class="tex-font-style-tt">Scanner/System.out</span> in <span class="tex-font-style-tt">Java</span>. Don't use the function <span class="tex-font-style-tt">input()</span> in <span class="tex-font-style-tt">Python2</span> instead of it use the function <span class="tex-font-style-tt">raw_input()</span>.</p></div><div class="input-specification"><p>The first line contains a non-negative integer <span class="tex-span"><i>a</i></span>.</p><p>The second line contains a non-negative integer <span class="tex-span"><i>b</i></span>.</p><p>The numbers <span class="tex-span"><i>a</i>, <i>b</i></span> may contain leading zeroes. Each of them contains no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> digits.</p></div><div class="output-specification"><p>Print the symbol "<span class="tex-font-style-tt">&lt;</span>" if <span class="tex-span"><i>a</i> &lt; <i>b</i></span> and the symbol "<span class="tex-font-style-tt">&gt;</span>" if <span class="tex-span"><i>a</i> &gt; <i>b</i></span>. If the numbers are equal print the symbol "<span class="tex-font-style-tt">=</span>".</p></div>

## Input

<p>The first line contains a non-negative integer <span class="tex-span"><i>a</i></span>.</p><p>The second line contains a non-negative integer <span class="tex-span"><i>b</i></span>.</p><p>The numbers <span class="tex-span"><i>a</i>, <i>b</i></span> may contain leading zeroes. Each of them contains no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> digits.</p>

## Output

<p>Print the symbol "<span class="tex-font-style-tt">&lt;</span>" if <span class="tex-span"><i>a</i> &lt; <i>b</i></span> and the symbol "<span class="tex-font-style-tt">&gt;</span>" if <span class="tex-span"><i>a</i> &gt; <i>b</i></span>. If the numbers are equal print the symbol "<span class="tex-font-style-tt">=</span>".</p>





```input1
9
10

```




```input2
11
10

```




```input3
00012345
12345

```




```input4
0123
9

```




```input5
0123
111

```




```output1
&lt;

```




```output2
&gt;

```




```output3
=

```




```output4
&gt;

```




```output5
&gt;

```


