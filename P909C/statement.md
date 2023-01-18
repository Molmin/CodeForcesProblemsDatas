## Description

<div><p>In Python, code blocks don't have explicit begin/end or curly braces to mark beginning and end of the block. Instead, code blocks are defined by indentation.</p><p>We will consider an extremely simplified subset of Python with only two types of statements.</p><p><span class="tex-font-style-bf">Simple statements</span> are written in a single line, one per line. An example of a simple statement is assignment.</p><p><span class="tex-font-style-bf">For statements</span> are compound statements: they contain one or several other statements. For statement consists of a header written in a separate line which starts with "for" prefix, and loop body. Loop body is a block of statements indented one level further than the header of the loop. Loop body can contain both types of statements. Loop body can't be empty.</p><p>You are given a sequence of statements without indentation. Find the number of ways in which the statements can be indented to form a valid Python program.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 5000</span>)&nbsp;— the number of commands in the program. <span class="tex-span"><i>N</i></span> lines of the program follow, each line describing a single command. Each command is either "f" (denoting "for statement") or "s" ("simple statement"). It is guaranteed that the last line is a simple statement.</p></div><div class="output-specification"><p>Output one line containing an integer - the number of ways the given sequence of statements can be indented modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 5000</span>)&nbsp;— the number of commands in the program. <span class="tex-span"><i>N</i></span> lines of the program follow, each line describing a single command. Each command is either "f" (denoting "for statement") or "s" ("simple statement"). It is guaranteed that the last line is a simple statement.</p>

## Output

<p>Output one line containing an integer - the number of ways the given sequence of statements can be indented modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </p>





```input1
4
s
f
f
s

```




```input2
4
f
s
f
s

```




```output1
1

```




```output2
2

```



## Note

<p>In the first test case, there is only one way to indent the program: the second for statement must be part of the body of the first one.</p><pre class="verbatim"><br>simple statement<br>for statement<br>    for statement<br>        simple statement<br></pre><p>In the second test case, there are two ways to indent the program: the second for statement can either be part of the first one's body or a separate statement following the first one.</p><pre class="verbatim"><br>for statement<br>    simple statement<br>    for statement<br>        simple statement<br></pre><p>or</p><pre class="verbatim"><br>for statement<br>    simple statement<br>for statement<br>    simple statement<br></pre>
