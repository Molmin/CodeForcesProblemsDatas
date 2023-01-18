## Description

<div><p>Iahub likes chess very much. He even invented a new chess piece named Coder. A Coder can move (and attack) one square horizontally or vertically. More precisely, if the Coder is located at position <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, he can move to (or attack) positions <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>–1, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span> and <span class="tex-span">(<i>x</i>, <i>y</i>–1)</span>.</p><p>Iahub wants to know how many Coders can be placed on an <span class="tex-span"><i>n</i> × <i>n</i></span> chessboard, so that no Coder attacks any other Coder.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span>.</p></div><div class="output-specification"><p>On the first line print an integer, the maximum number of Coders that can be placed on the chessboard.</p><p>On each of the next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>n</i></span> characters, describing the configuration of the Coders. For an empty cell print an '<span class="tex-font-style-tt">.</span>', and for a Coder print a '<span class="tex-font-style-tt">C</span>'.</p><p>If there are multiple correct answers, you can print any.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span>.</p>

## Output

<p>On the first line print an integer, the maximum number of Coders that can be placed on the chessboard.</p><p>On each of the next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>n</i></span> characters, describing the configuration of the Coders. For an empty cell print an '<span class="tex-font-style-tt">.</span>', and for a Coder print a '<span class="tex-font-style-tt">C</span>'.</p><p>If there are multiple correct answers, you can print any.</p>





```input1
2

```




```output1
2
C.
.C

```


