## Description

<div><p>Polycarp has a string $s[1 \dots n]$ of length $n$ consisting of decimal digits. Polycarp performs the following operation with the string $s$ <span class="tex-font-style-bf">no more than once</span> (i.e. he can perform operation $0$ or $1$ time): </p><ul> <li> Polycarp selects two numbers $i$ and $j$ ($1 \leq i \leq j \leq n$) and removes characters from the $s$ string at the positions $i, i+1, i+2, \ldots, j$ (i.e. removes substring $s[i \dots j]$). More formally, Polycarp turns the string $s$ into the string $s_1 s_2 \ldots s_{i-1} s_{j+1} s_{j+2} \ldots s_{n}$. </li></ul><p>For example, the string $s = $"<span class="tex-font-style-tt">20192020</span>" Polycarp can turn into strings: </p><ul> <li> "<span class="tex-font-style-tt">2020</span>" (in this case $(i, j)=(3, 6)$ or $(i, j)=(1, 4)$); </li><li> "<span class="tex-font-style-tt">2019220</span>" (in this case $(i, j)=(6, 6)$); </li><li> "<span class="tex-font-style-tt">020</span>" (in this case $(i, j)=(1, 5)$); </li><li> other operations are also possible, only a few of them are listed above. </li></ul><p>Polycarp likes the string "<span class="tex-font-style-tt">2020</span>" very much, so he is wondering if it is possible to turn the string $s$ into a string "<span class="tex-font-style-tt">2020</span>" in no more than one operation? Note that you can perform zero operations.</p></div><div class="input-specification"><p>The first line contains a positive integer $t$ ($1 \leq t \leq 1000 $)&nbsp;— number of test cases in the test. Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($4 \leq n \leq 200$)&nbsp;— length of the string $s$. The next line contains a string $s$ of length $n$ consisting of decimal digits. It is allowed that the string $s$ starts with digit <span class="tex-font-style-tt">0</span>.</p></div><div class="output-specification"><p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" if Polycarp can turn the string $s$ into a string "<span class="tex-font-style-tt">2020</span>" in no more than one operation (i.e. he can perform $0$ or $1$ operation); </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You may print every letter of "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p></div>

## Input

<p>The first line contains a positive integer $t$ ($1 \leq t \leq 1000 $)&nbsp;— number of test cases in the test. Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($4 \leq n \leq 200$)&nbsp;— length of the string $s$. The next line contains a string $s$ of length $n$ consisting of decimal digits. It is allowed that the string $s$ starts with digit <span class="tex-font-style-tt">0</span>.</p>

## Output

<p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" if Polycarp can turn the string $s$ into a string "<span class="tex-font-style-tt">2020</span>" in no more than one operation (i.e. he can perform $0$ or $1$ operation); </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You may print every letter of "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p>





```input1
6
8
20192020
8
22019020
4
2020
5
20002
6
729040
6
200200
```




```output1
YES
YES
YES
NO
NO
NO
```



## Note

<p>In the first test case, Polycarp could choose $i=3$ and $j=6$.</p><p>In the second test case, Polycarp could choose $i=2$ and $j=5$.</p><p>In the third test case, Polycarp did not perform any operations with the string.</p>
