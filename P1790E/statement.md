## Description

<div><p>Vlad found two positive numbers $a$ and $b$ ($a,b&gt;0$). He discovered that $a \oplus b = \frac{a + b}{2}$, where $\oplus$ means the <a href="http://tiny.cc/xor_wiki_eng">bitwise exclusive OR</a> , and division is performed without rounding..</p><p>Since it is easier to remember one number than two, Vlad remembered only $a\oplus b$, let's denote this number as $x$. Help him find any suitable $a$ and $b$ or tell him that they do not exist.</p></div><div class="input-specification"><p>The first line of the input data contains the single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test. </p><p>Each test case is described by a single integer $x$ ($1 \le x \le 2^{29}$)&nbsp;— the number that Vlad remembered.</p></div><div class="output-specification"><p>Output $t$ lines, each of which is the answer to the corresponding test case. As the answer, output $a$ and $b$ ($0 &lt; a,b \le 2^{32}$), such that $x = a \oplus b = \frac{a + b}{2}$. If there are several answers, output any of them. If there are no matching pairs, output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line of the input data contains the single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test. </p><p>Each test case is described by a single integer $x$ ($1 \le x \le 2^{29}$)&nbsp;— the number that Vlad remembered.</p>

## Output

<p>Output $t$ lines, each of which is the answer to the corresponding test case. As the answer, output $a$ and $b$ ($0 &lt; a,b \le 2^{32}$), such that $x = a \oplus b = \frac{a + b}{2}$. If there are several answers, output any of them. If there are no matching pairs, output <span class="tex-font-style-tt">-1</span>.</p>





```input1|2,4,6
6
2
5
10
6
18
36
```




```output1
3 1
-1
13 7
-1
25 11
50 22
```


