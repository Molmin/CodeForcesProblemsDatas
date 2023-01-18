## Description

<div><p>Let's define an <span class="tex-font-style-it">unambiguous arithmetic expression</span> (UAE) as follows. </p><ul> <li> All non-negative integers are UAE's. Integers may have leading zeroes (for example, <span class="tex-span">0000</span> and <span class="tex-span">0010</span> are considered valid integers). </li><li> If <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> are two UAE's, then "<span class="tex-span">(<i>X</i>) + (<i>Y</i>)</span>", "<span class="tex-span">(<i>X</i>) - (<i>Y</i>)</span>", "<span class="tex-span">(<i>X</i>) * (<i>Y</i>)</span>", and "<span class="tex-span">(<i>X</i>) / (<i>Y</i>)</span>" (all without the double quotes) are UAE's. </li><li> If <span class="tex-span"><i>X</i></span> is an UAE, then "<span class="tex-span"> - (<i>X</i>)</span>" and "<span class="tex-span"> + (<i>X</i>)</span>" (both without the double quotes) are UAE's.<p>You are given a string consisting only of digits ("<span class="tex-font-style-tt">0</span>" - "<span class="tex-font-style-tt">9</span>") and characters "<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">+</span>", "<span class="tex-font-style-tt">*</span>", and "<span class="tex-font-style-tt">/</span>". Your task is to compute the number of different possible unambiguous arithmetic expressions such that if all brackets (characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>") of that unambiguous arithmetic expression are removed, it becomes the input string. Since the answer may be very large, print it modulo <span class="tex-span">1000003</span> (<span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>).</p></li></ul></div><div class="input-specification"><p>The first line is a <span class="tex-font-style-underline">non-empty</span> string consisting of digits ('0'-'9') and characters '-', '+', '*', and/or '/'. Its length will not exceed <span class="tex-span">2000</span>. The line doesn't contain any spaces.</p></div><div class="output-specification"><p>Print a single integer representing the number of different unambiguous arithmetic expressions modulo <span class="tex-span">1000003</span> (<span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>) such that if all its brackets are removed, it becomes equal to the input string (character-by-character).</p></div>

## Input

<p>The first line is a <span class="tex-font-style-underline">non-empty</span> string consisting of digits ('0'-'9') and characters '-', '+', '*', and/or '/'. Its length will not exceed <span class="tex-span">2000</span>. The line doesn't contain any spaces.</p>

## Output

<p>Print a single integer representing the number of different unambiguous arithmetic expressions modulo <span class="tex-span">1000003</span> (<span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>) such that if all its brackets are removed, it becomes equal to the input string (character-by-character).</p>





```input1
1+2*3

```




```input2
03+-30+40

```




```input3
5//4

```




```input4
5/0

```




```input5
1+1+1+1+1+1+1+1+1+1+1+1+1+1+1+1+1+1+1+1+1

```




```output1
2

```




```output2
3

```




```output3
0

```




```output4
1

```




```output5
100728

```



## Note

<p>For the first example, the two possible unambiguous arithmetic expressions are:</p><pre class="verbatim"><span class="tex-span">((1) + (2)) * (3)</span><br><span class="tex-span">(1) + ((2) * (3))</span></pre><p>For the second example, the three possible unambiguous arithmetic expressions are:</p><pre class="verbatim"><span class="tex-span">(03) + (( - (30)) + (40))</span><br><span class="tex-span">(03) + ( - ((30) + (40)))</span><br><span class="tex-span">((03) + ( - (30))) + (40)</span></pre>
