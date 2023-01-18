## Description

<div><p>Let's analyze a program written on some strange programming language. The variables in this language have names consisting of $1$ to $4$ characters, and each character is a lowercase or an uppercase Latin letter, or a digit. There is an extra constraint that the first character should not be a digit.</p><p>There are four types of operations in the program, each denoted by one of the characters: <span class="tex-font-style-tt">$</span>, <span class="tex-font-style-tt">^</span>, <span class="tex-font-style-tt">#</span> or <span class="tex-font-style-tt">&amp;</span>.</p><p>Each line of the program has one of the following formats: </p><ul> <li> <span class="tex-font-style-tt">&lt;lvalue&gt;=&lt;rvalue&gt;</span>, where <span class="tex-font-style-tt">&lt;lvalue&gt;</span> and <span class="tex-font-style-tt">&lt;rvalue&gt;</span> are valid variable names; </li><li> <span class="tex-font-style-tt">&lt;lvalue&gt;=&lt;arg1&gt;&lt;op&gt;&lt;arg2&gt;</span>, where <span class="tex-font-style-tt">&lt;lvalue&gt;</span>, <span class="tex-font-style-tt">&lt;arg1&gt;</span> and <span class="tex-font-style-tt">&lt;arg2&gt;</span> are valid variable names, and &lt;op&gt; is an operation character. </li></ul><p>The program is executed line-by-line, and the result of execution is stored in a variable having the name <span class="tex-font-style-tt">res</span>. If <span class="tex-font-style-tt">res</span> is never assigned in the program, then the result will be equal to the value of <span class="tex-font-style-tt">res</span> before running the program.</p><p>Two programs are called equivalent if no matter which operations do characters <span class="tex-font-style-tt">$</span>, <span class="tex-font-style-tt">^</span>, <span class="tex-font-style-tt">#</span> and <span class="tex-font-style-tt">&amp;</span> denote (but, obviously, performing the same operation on the same arguments gives the same result) and which values do variables have before execution of program, the value of <span class="tex-font-style-tt">res</span> after running the first program is equal to the value of <span class="tex-font-style-tt">res</span> after running the second program (the programs are executed independently).</p><p>You are given a program consisting of $n$ lines. Your task is to write a program consisting of minimum possible number of lines that is equivalent to the program you are given.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 1000$) — the number of lines in the program.</p><p>Then $n$ lines follow — the program itself. Each line corresponds to the format described in the statement and has no extra whitespaces.</p></div><div class="output-specification"><p>In the first line print $k$ — the minimum number of lines in the equivalent program.</p><p>Then print $k$ lines without any whitespaces — an equivalent program having exactly $k$ lines, in the same format it is described in the statement.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 1000$) — the number of lines in the program.</p><p>Then $n$ lines follow — the program itself. Each line corresponds to the format described in the statement and has no extra whitespaces.</p>

## Output

<p>In the first line print $k$ — the minimum number of lines in the equivalent program.</p><p>Then print $k$ lines without any whitespaces — an equivalent program having exactly $k$ lines, in the same format it is described in the statement.</p>





```input1
4
c=aa#bb
d12=c
res=c^d12
tmp=aa$c
```




```input2
2
max=aaaa$bbbb
min=bbbb^aaaa
```




```output1
2
aaaa=aa#bb
res=aaaa^aaaa
```




```output2
0
```


