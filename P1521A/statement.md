## Description

<div><p>Nastia has $2$ positive integers $A$ and $B$. She defines that:</p><ul> <li> The integer is good if it is divisible by $A \cdot B$; </li><li> Otherwise, the integer is nearly good, if it is divisible by $A$. </li></ul><p>For example, if $A = 6$ and $B = 4$, the integers $24$ and $72$ are good, the integers $6$, $660$ and $12$ are nearly good, the integers $16$, $7$ are neither good nor nearly good.</p><p>Find $3$ <span class="tex-font-style-bf">different</span> positive integers $x$, $y$, and $z$ such that <span class="tex-font-style-bf">exactly one</span> of them is good and the <span class="tex-font-style-bf">other</span> $2$ are nearly good, and $x + y = z$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $A$ and $B$ ($1 \le A \le 10^6$, $1 \le B \le 10^6$)&nbsp;— numbers that Nastia has.</p></div><div class="output-specification"><p>For each test case print: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" and $3$ <span class="tex-font-style-bf">different</span> positive integers $x$, $y$, and $z$ ($1 \le x, y, z \le 10^{18}$) such that <span class="tex-font-style-bf">exactly one</span> of them is good and the <span class="tex-font-style-bf">other</span> $2$ are nearly good, and $x + y = z$. </li><li> "<span class="tex-font-style-tt">NO</span>" if no answer exists. </li></ul> You can print each character of "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" in any case.<p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $A$ and $B$ ($1 \le A \le 10^6$, $1 \le B \le 10^6$)&nbsp;— numbers that Nastia has.</p>

## Output

<p>For each test case print: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" and $3$ <span class="tex-font-style-bf">different</span> positive integers $x$, $y$, and $z$ ($1 \le x, y, z \le 10^{18}$) such that <span class="tex-font-style-bf">exactly one</span> of them is good and the <span class="tex-font-style-bf">other</span> $2$ are nearly good, and $x + y = z$. </li><li> "<span class="tex-font-style-tt">NO</span>" if no answer exists. </li></ul> You can print each character of "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" in any case.<p>If there are multiple answers, print any.</p>





```input1
3
5 3
13 2
7 11
```




```output1
YES
10 50 60
YES
169 39 208
YES
28 154 182
```



## Note

<p>In the first test case: $60$&nbsp;— good number; $10$ and $50$&nbsp;— nearly good numbers.</p><p>In the second test case: $208$&nbsp;— good number; $169$ and $39$&nbsp;— nearly good numbers.</p><p>In the third test case: $154$&nbsp;— good number; $28$ and $182$&nbsp;— nearly good numbers.</p>
