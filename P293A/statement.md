## Description

<div><p>Yaroslav, Andrey and Roman can play cubes for hours and hours. But the game is for three, so when Roman doesn't show up, Yaroslav and Andrey play another game. </p><p>Roman leaves a word for each of them. Each word consists of <span class="tex-span">2·<i>n</i></span> binary characters "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>". After that the players start moving in turns. Yaroslav moves first. During a move, a player must choose an integer from 1 to <span class="tex-span">2·<i>n</i></span>, which hasn't been chosen by anybody up to that moment. Then the player takes a piece of paper and writes out the corresponding character from his string. </p><p>Let's represent Yaroslav's word as <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">2<i>n</i></sub></span>. Similarly, let's represent Andrey's word as <span class="tex-span"><i>t</i> = <i>t</i><sub class="lower-index">1</sub><i>t</i><sub class="lower-index">2</sub>... <i>t</i><sub class="lower-index">2<i>n</i></sub></span>. Then, if Yaroslav choose number <span class="tex-span"><i>k</i></span> during his move, then he is going to write out character <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span> on the piece of paper. Similarly, if Andrey choose number <span class="tex-span"><i>r</i></span> during his move, then he is going to write out character <span class="tex-span"><i>t</i><sub class="lower-index"><i>r</i></sub></span> on the piece of paper.</p><p>The game finishes when no player can make a move. After the game is over, Yaroslav makes some integer from the characters written on his piece of paper (Yaroslav can arrange these characters as he wants). Andrey does the same. The resulting numbers can contain leading zeroes. The person with the largest number wins. If the numbers are equal, the game ends with a draw.</p><p>You are given two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. Determine the outcome of the game provided that Yaroslav and Andrey play optimally well.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). The second line contains string <span class="tex-span"><i>s</i></span> — Yaroslav's word. The third line contains string <span class="tex-span"><i>t</i></span> — Andrey's word.</p><p>It is guaranteed that both words consist of <span class="tex-span">2·<i>n</i></span> characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>".</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">First</span>", if both players play optimally well and Yaroslav wins. If Andrey wins, print "<span class="tex-font-style-tt">Second</span>" and if the game ends with a draw, print "<span class="tex-font-style-tt">Draw</span>". Print the words without the quotes.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). The second line contains string <span class="tex-span"><i>s</i></span> — Yaroslav's word. The third line contains string <span class="tex-span"><i>t</i></span> — Andrey's word.</p><p>It is guaranteed that both words consist of <span class="tex-span">2·<i>n</i></span> characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>".</p>

## Output

<p>Print "<span class="tex-font-style-tt">First</span>", if both players play optimally well and Yaroslav wins. If Andrey wins, print "<span class="tex-font-style-tt">Second</span>" and if the game ends with a draw, print "<span class="tex-font-style-tt">Draw</span>". Print the words without the quotes.</p>





```input1
2
0111
0001

```




```input2
3
110110
001001

```




```input3
3
111000
000111

```




```input4
4
01010110
00101101

```




```input5
4
01100000
10010011

```




```output1
First

```




```output2
First

```




```output3
Draw

```




```output4
First

```




```output5
Second

```


