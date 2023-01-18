## Description

<div><p>There is a string <span class="tex-span"><i>s</i></span>, consisting of capital Latin letters. Let's denote its current length as <span class="tex-span">|<i>s</i>|</span>. During one move it is allowed to apply one of the following operations to it: </p><ul> <li> <span class="tex-font-style-tt">INSERT</span> <span class="tex-span"><i>pos</i></span> <span class="tex-span"><i>ch</i></span> — insert a letter <span class="tex-span"><i>ch</i></span> in the string <span class="tex-span"><i>s</i></span> in the position <span class="tex-span"><i>pos</i></span> (<span class="tex-span">1 ≤ <i>pos</i> ≤ |<i>s</i>| + 1, <i>A</i> ≤ <i>ch</i> ≤ <i>Z</i></span>). The letter <span class="tex-span"><i>ch</i></span> becomes the <span class="tex-span"><i>pos</i></span>-th symbol of the string <span class="tex-span"><i>s</i></span>, at that the letters shift aside and the length of the string increases by 1. </li><li> <span class="tex-font-style-tt">DELETE</span> <span class="tex-span"><i>pos</i></span> — delete a character number <span class="tex-span"><i>pos</i></span> (<span class="tex-span">1 ≤ <i>pos</i> ≤ |<i>s</i>|</span>) from the string <span class="tex-span"><i>s</i></span>. At that the letters shift together and the length of the string decreases by 1. </li><li> <span class="tex-font-style-tt">REPLACE</span> <span class="tex-span"><i>pos</i></span> <span class="tex-span"><i>ch</i></span> — the letter in the position <span class="tex-span"><i>pos</i></span> of the line <span class="tex-span"><i>s</i></span> is replaced by <span class="tex-span"><i>ch</i></span> (<span class="tex-span">1 ≤ <i>pos</i> ≤ |<i>s</i>|, <i>A</i> ≤ <i>ch</i> ≤ <i>Z</i></span>). At that the length of the string does not change. </li></ul><p>Your task is to find in which minimal number of moves one can get a <span class="tex-span"><i>t</i></span> string from an <span class="tex-span"><i>s</i></span> string. You should also find the sequence of actions leading to the required results.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>s</i></span>, the second line contains <span class="tex-span"><i>t</i></span>. The lines consist only of capital Latin letters, their lengths are positive numbers from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>In the first line print the number of moves <span class="tex-span"><i>k</i></span> in the given sequence of operations. The number should be the minimal possible one. Then print <span class="tex-span"><i>k</i></span> lines containing one operation each. Print the operations in the format, described above. If there are several solutions, print any of them.</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>s</i></span>, the second line contains <span class="tex-span"><i>t</i></span>. The lines consist only of capital Latin letters, their lengths are positive numbers from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p>

## Output

<p>In the first line print the number of moves <span class="tex-span"><i>k</i></span> in the given sequence of operations. The number should be the minimal possible one. Then print <span class="tex-span"><i>k</i></span> lines containing one operation each. Print the operations in the format, described above. If there are several solutions, print any of them.</p>





```input1
ABA
ABBBA

```




```input2
ACCEPTED
WRONGANSWER

```




```output1
2
INSERT 3 B
INSERT 4 B

```




```output2
10
REPLACE 1 W
REPLACE 2 R
REPLACE 3 O
REPLACE 4 N
REPLACE 5 G
REPLACE 6 A
INSERT 7 N
INSERT 8 S
INSERT 9 W
REPLACE 11 R

```


