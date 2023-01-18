## Description

<div><p>Implication is a function of two logical arguments, its value is false if and only if the value of the first argument is true and the value of the second argument is false. </p><p>Implication is written by using character '<span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="file://9ausTuud.png" style="max-width: 100.0%;max-height: 100.0%;"></span>', and the arguments and the result of the implication are written as '<span class="tex-font-style-tt">0</span>' (<span class="tex-span"><i>false</i></span>) and '<span class="tex-font-style-tt">1</span>' (<span class="tex-span"><i>true</i></span>). According to the definition of the implication: </p><center><p><img align="middle" class="tex-formula" src="file://hb9k49cL.png" style="max-width: 100.0%;max-height: 100.0%;"> </p><p><img align="middle" class="tex-formula" src="file://bxU0z78B.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://rNUR5aO7.png" style="max-width: 100.0%;max-height: 100.0%;"> </p><p><img align="middle" class="tex-formula" src="file://NwwXaQL0.png" style="max-width: 100.0%;max-height: 100.0%;"></p></center><p>When a logical expression contains multiple implications, then when there are no brackets, it will be calculated from left to fight. For example,</p><p><img align="middle" class="tex-formula" src="file://4I7vwFEB.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>When there are brackets, we first calculate the expression in brackets. For example,</p><p><img align="middle" class="tex-formula" src="file://GCH5bc6F.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>For the given logical expression <img align="middle" class="tex-formula" src="file://LloxzOCC.png" style="max-width: 100.0%;max-height: 100.0%;"> determine if it is possible to place there brackets so that the value of a logical expression is false. If it is possible, your task is to find such an arrangement of brackets.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of arguments in a logical expression.</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://h7B1DFZj.png" style="max-width: 100.0%;max-height: 100.0%;">), which means the values of arguments in the expression in the order they occur.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" (without the quotes), if it is impossible to place brackets in the expression so that its value was equal to 0.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and the logical expression with the required arrangement of brackets in the second line.</p><p>The expression should only contain characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>', '<span class="tex-font-style-tt">-</span>' (character with ASCII code 45), '<span class="tex-font-style-tt">&gt;</span>' (character with ASCII code 62), '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'. Characters '<span class="tex-font-style-tt">-</span>' and '<span class="tex-font-style-tt">&gt;</span>' can occur in an expression only paired like that: ("<span class="tex-font-style-tt">-&gt;</span>") and represent implication. The total number of logical arguments (i.e. digits '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>') in the expression must be equal to <span class="tex-span"><i>n</i></span>. The order in which the digits follow in the expression from left to right must coincide with <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>The expression should be <span class="tex-font-style-it">correct</span>. More formally, a <span class="tex-font-style-it">correct</span> expression is determined as follows:</p><ul> <li> Expressions "<span class="tex-span">0</span>", "<span class="tex-span">1</span>" (without the quotes) are correct. </li><li> If <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> are correct, then <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span><span class="tex-font-style-tt">-&gt;</span><span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> is a correct expression. </li><li> If <span class="tex-span"><i>v</i></span> is a correct expression, then <span class="tex-span">(<i>v</i>)</span> is a correct expression. </li></ul><p>The total number of characters in the resulting expression mustn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>If there are multiple possible answers, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the number of arguments in a logical expression.</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<img align="middle" class="tex-formula" src="file://h7B1DFZj.png" style="max-width: 100.0%;max-height: 100.0%;">), which means the values of arguments in the expression in the order they occur.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" (without the quotes), if it is impossible to place brackets in the expression so that its value was equal to 0.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and the logical expression with the required arrangement of brackets in the second line.</p><p>The expression should only contain characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>', '<span class="tex-font-style-tt">-</span>' (character with ASCII code 45), '<span class="tex-font-style-tt">&gt;</span>' (character with ASCII code 62), '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'. Characters '<span class="tex-font-style-tt">-</span>' and '<span class="tex-font-style-tt">&gt;</span>' can occur in an expression only paired like that: ("<span class="tex-font-style-tt">-&gt;</span>") and represent implication. The total number of logical arguments (i.e. digits '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>') in the expression must be equal to <span class="tex-span"><i>n</i></span>. The order in which the digits follow in the expression from left to right must coincide with <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>The expression should be <span class="tex-font-style-it">correct</span>. More formally, a <span class="tex-font-style-it">correct</span> expression is determined as follows:</p><ul> <li> Expressions "<span class="tex-span">0</span>", "<span class="tex-span">1</span>" (without the quotes) are correct. </li><li> If <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> are correct, then <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span><span class="tex-font-style-tt">-&gt;</span><span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> is a correct expression. </li><li> If <span class="tex-span"><i>v</i></span> is a correct expression, then <span class="tex-span">(<i>v</i>)</span> is a correct expression. </li></ul><p>The total number of characters in the resulting expression mustn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>If there are multiple possible answers, you are allowed to print any of them.</p>





```input1
4
0 1 1 0

```




```input2
2
1 1

```




```input3
1
0

```




```output1
YES
(((0)-&gt;1)-&gt;(1-&gt;0))

```




```output2
NO

```




```output3
YES
0

```


