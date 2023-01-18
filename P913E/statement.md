## Description

<div><p>You are given a boolean function of three variables which is defined by its truth table. You need to find an expression of minimum length that equals to this function. The expression may consist of: </p><ul> <li> Operation <span class="tex-font-style-tt">AND</span> ('<span class="tex-font-style-tt">&amp;</span>', ASCII code 38) </li><li> Operation <span class="tex-font-style-tt">OR</span> ('<span class="tex-font-style-tt">|</span>', ASCII code 124) </li><li> Operation <span class="tex-font-style-tt">NOT</span> ('<span class="tex-font-style-tt">!</span>', ASCII code 33) </li><li> Variables <span class="tex-font-style-tt">x</span>, <span class="tex-font-style-tt">y</span> and <span class="tex-font-style-tt">z</span> (ASCII codes 120-122) </li><li> Parentheses ('<span class="tex-font-style-tt">(</span>', ASCII code 40, and '<span class="tex-font-style-tt">)</span>', ASCII code 41) </li></ul><p>If more than one expression of minimum length exists, you should find the lexicographically smallest one.</p><p>Operations have standard priority. <span class="tex-font-style-tt">NOT</span> has the highest priority, then <span class="tex-font-style-tt">AND</span> goes, and <span class="tex-font-style-tt">OR</span> has the lowest priority. The expression should satisfy the following grammar:</p><p>E ::= E '<span class="tex-font-style-tt">|</span>' T | T</p><p>T ::= T '<span class="tex-font-style-tt">&amp;</span>' F | F</p><p>F ::= '<span class="tex-font-style-tt">!</span>' F | '<span class="tex-font-style-tt">(</span>' E '<span class="tex-font-style-tt">)</span>' | '<span class="tex-font-style-tt">x</span>' | '<span class="tex-font-style-tt">y</span>' | '<span class="tex-font-style-tt">z</span>'</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of functions in the input (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>).</p><p>The following <span class="tex-span"><i>n</i></span> lines contain descriptions of functions, the <span class="tex-span"><i>i</i></span>-th of them contains a string of length <span class="tex-span">8</span> that consists of digits <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>&nbsp;— the truth table of the <span class="tex-span"><i>i</i></span>-th function. The digit on position <span class="tex-span"><i>j</i></span> (<span class="tex-span">0 ≤ <i>j</i> &lt; 8</span>) equals to the value of the function in case of <img align="middle" class="tex-formula" src="file://qI12mkmB.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://arWHPMl1.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://XEvRKCtr.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>You should output <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain the expression of minimum length which equals to the <span class="tex-span"><i>i</i></span>-th function. If there is more than one such expression, output the lexicographically smallest of them. Expressions should satisfy the given grammar and shouldn't contain white spaces.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of functions in the input (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>).</p><p>The following <span class="tex-span"><i>n</i></span> lines contain descriptions of functions, the <span class="tex-span"><i>i</i></span>-th of them contains a string of length <span class="tex-span">8</span> that consists of digits <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>&nbsp;— the truth table of the <span class="tex-span"><i>i</i></span>-th function. The digit on position <span class="tex-span"><i>j</i></span> (<span class="tex-span">0 ≤ <i>j</i> &lt; 8</span>) equals to the value of the function in case of <img align="middle" class="tex-formula" src="file://qI12mkmB.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://arWHPMl1.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://XEvRKCtr.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>You should output <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain the expression of minimum length which equals to the <span class="tex-span"><i>i</i></span>-th function. If there is more than one such expression, output the lexicographically smallest of them. Expressions should satisfy the given grammar and shouldn't contain white spaces.</p>





```input1
4
00110011
00000111
11110000
00011111

```




```output1
y
(y|z)&amp;x
!x
x|y&amp;z

```



## Note

<p>The truth table for the second function:</p><p><img class="tex-graphics" src="file://WFz7Gjl0.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
