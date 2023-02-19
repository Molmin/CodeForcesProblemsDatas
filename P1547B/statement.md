## Description

<div><p>A string $s$ of length $n$ ($1 \le n \le 26$) is called <span class="tex-font-style-it">alphabetical</span> if it can be obtained using the following algorithm:</p><ul> <li> first, write an empty string to $s$ (i.e. perform the assignment $s$&nbsp;<span class="tex-font-style-tt">:= ""</span>); </li><li> then perform the next step $n$ times; </li><li> at the $i$-th step take $i$-th lowercase letter of the Latin alphabet and write it either to the left of the string $s$ or to the right of the string $s$ (i.e. perform the assignment $s$&nbsp;<span class="tex-font-style-tt">:=</span>&nbsp;$c+s$ or $s$&nbsp;<span class="tex-font-style-tt">:=</span>&nbsp;$s+c$, where $c$ is the $i$-th letter of the Latin alphabet). </li></ul><p>In other words, iterate over the $n$ first letters of the Latin alphabet starting from '<span class="tex-font-style-tt">a</span>' and etc. Each time we prepend a letter to the left of the string $s$ or append a letter to the right of the string $s$. Strings that can be obtained in that way are alphabetical.</p><p>For example, the following strings are alphabetical: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">bac</span>" and "<span class="tex-font-style-tt">ihfcbadeg</span>". The following strings <span class="tex-font-style-bf">are not</span> alphabetical: "<span class="tex-font-style-tt">z</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ca</span>", "<span class="tex-font-style-tt">acb</span>", "<span class="tex-font-style-tt">xyz</span>" and "<span class="tex-font-style-tt">ddcba</span>".</p><p>From the given string, determine if it is alphabetical.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case is written on a separate line that contains one string $s$. String $s$ consists of lowercase letters of the Latin alphabet and has a length between $1$ and $26$, inclusive.</p></div><div class="output-specification"><p>Output $t$ lines, each of them must contain the answer to the corresponding test case. Output <span class="tex-font-style-tt">YES</span> if the given string $s$ is alphabetical and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case is written on a separate line that contains one string $s$. String $s$ consists of lowercase letters of the Latin alphabet and has a length between $1$ and $26$, inclusive.</p>

## Output

<p>Output $t$ lines, each of them must contain the answer to the corresponding test case. Output <span class="tex-font-style-tt">YES</span> if the given string $s$ is alphabetical and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer).</p>





```input1
11
a
ba
ab
bac
ihfcbadeg
z
aa
ca
acb
xyz
ddcba
```




```output1
YES
YES
YES
YES
YES
NO
NO
NO
NO
NO
NO
```



## Note

<p>The example contains test cases from the main part of the condition.</p>
