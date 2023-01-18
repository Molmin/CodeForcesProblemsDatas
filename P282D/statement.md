## Description

<div><p>Since most contestants do not read this part, I have to repeat that Bitlandians are quite weird. They have their own jobs, their own working method, their own lives, their own sausages and their own games!</p><p>Since you are so curious about Bitland, I'll give you the chance of peeking at one of these games.</p><p>BitLGM and BitAryo are playing yet another of their crazy-looking genius-needed Bitlandish games. They've got a sequence of <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. The players make moves in turns. BitLGM moves first. Each player can and must do one of the two following actions in his turn:</p><ul> <li> Take one of the integers (we'll denote it as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>). Choose integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>)</span>. And then decrease <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>x</i></span>, that is, apply assignment: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub> - <i>x</i></span>. </li><li> Choose integer <span class="tex-span"><i>x</i></span> <img align="middle" class="tex-formula" src="file://hBCT3Frm.png" style="max-width: 100.0%;max-height: 100.0%;">. And then decrease all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>x</i></span>, that is, apply assignment: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub> - <i>x</i></span>, for all <span class="tex-span"><i>i</i></span>. </li></ul><p>The player who cannot make a move loses.</p><p>You're given the initial sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Determine who wins, if both players plays optimally well and if BitLGM and BitAryo start playing the described game in this sequence.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3</span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 300)</span>.</p></div><div class="output-specification"><p>Write the name of the winner (provided that both players play optimally well). Either "<span class="tex-font-style-tt">BitLGM</span>" or "<span class="tex-font-style-tt">BitAryo</span>" (without the quotes).</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3</span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 300)</span>.</p>

## Output

<p>Write the name of the winner (provided that both players play optimally well). Either "<span class="tex-font-style-tt">BitLGM</span>" or "<span class="tex-font-style-tt">BitAryo</span>" (without the quotes).</p>





```input1
2
1 1

```




```input2
2
1 2

```




```input3
3
1 2 1

```




```output1
BitLGM

```




```output2
BitAryo

```




```output3
BitLGM

```


