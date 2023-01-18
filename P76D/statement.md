## Description

<div><p>Bitwise exclusive OR (or bitwise addition modulo two) is a binary operation which is equivalent to applying logical exclusive OR to every pair of bits located on the same positions in binary notation of operands. In other words, a binary digit of the result is equal to 1 if and only if bits on the respective positions in the operands are different.</p><p>For example, if <span class="tex-span"><i>X</i> = 109<sub class="lower-index">10</sub> = 1101101<sub class="lower-index">2</sub></span>, <span class="tex-span"><i>Y</i> = 41<sub class="lower-index">10</sub> = 101001<sub class="lower-index">2</sub></span>, then: </p><center> <span class="tex-span"><i>X</i></span> <span class="tex-font-style-tt">xor</span> <span class="tex-span"><i>Y</i>&nbsp; = &nbsp;68<sub class="lower-index">10</sub>&nbsp; = &nbsp;1000100<sub class="lower-index">2</sub></span>. </center><p>Write a program, which takes two non-negative integers <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> as an input and finds two non-negative integers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span>, which satisfy the following conditions: </p><ul> <li> <span class="tex-span"><i>A</i> = <i>X</i> + <i>Y</i></span> </li><li> <span class="tex-span"><i>B</i>&nbsp; = &nbsp;<i>X</i></span> <span class="tex-font-style-tt">xor</span> <span class="tex-span"><i>Y</i></span>, where <span class="tex-font-style-tt">xor</span> is bitwise exclusive or. </li><li> <span class="tex-span"><i>X</i></span> is the smallest number among all numbers for which the first two conditions are true. </li></ul></div><div class="input-specification"><p>The first line contains integer number <span class="tex-span"><i>A</i></span> and the second line contains integer number <span class="tex-span"><i>B</i></span> (<span class="tex-span">0 ≤ <i>A</i>, <i>B</i> ≤ 2<sup class="upper-index">64</sup> - 1</span>).</p></div><div class="output-specification"><p>The only output line should contain two integer non-negative numbers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span>. Print the only number <span class="tex-font-style-tt">-1</span> if there is no answer.</p></div>

## Input

<p>The first line contains integer number <span class="tex-span"><i>A</i></span> and the second line contains integer number <span class="tex-span"><i>B</i></span> (<span class="tex-span">0 ≤ <i>A</i>, <i>B</i> ≤ 2<sup class="upper-index">64</sup> - 1</span>).</p>

## Output

<p>The only output line should contain two integer non-negative numbers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span>. Print the only number <span class="tex-font-style-tt">-1</span> if there is no answer.</p>





```input1
142
76

```




```output1
33 109

```


