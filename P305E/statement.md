## Description

<div><p>Two people play the following string game. Initially the players have got some string <span class="tex-span"><i>s</i></span>. The players move in turns, the player who cannot make a move loses. </p><p>Before the game began, the string is written on a piece of paper, one letter per cell.</p><center> <img class="tex-graphics" src="file://r1lbFmwn.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script">An example of the initial situation at <span class="tex-span"><i>s</i></span> = "<span class="tex-font-style-tt">abacaba</span>"</span> </center><p>A player's move is the sequence of actions:</p><ol> <li> The player chooses one of the available pieces of paper with some string written on it. Let's denote it is <span class="tex-span"><i>t</i></span>. Note that initially, only one piece of paper is available. </li><li> The player chooses in the string <span class="tex-span"><i>t</i> = <i>t</i><sub class="lower-index">1</sub><i>t</i><sub class="lower-index">2</sub>... <i>t</i><sub class="lower-index">|<i>t</i>|</sub></span> character in position <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ |<i>t</i>|)</span> such that for some positive integer <span class="tex-span"><i>l</i></span> <span class="tex-span">(0 &lt; <i>i</i> - <i>l</i>;&nbsp;<i>i</i> + <i>l</i> ≤ |<i>t</i>|)</span> the following equations hold: <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> - 1</sub> = <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> - 2</sub> = <i>t</i><sub class="lower-index"><i>i</i> + 2</sub></span>, ..., <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> - <i>l</i></sub> = <i>t</i><sub class="lower-index"><i>i</i> + <i>l</i></sub></span>. </li><li> Player cuts the cell with the chosen character. As a result of the operation, he gets three new pieces of paper, the first one will contain string <span class="tex-span"><i>t</i><sub class="lower-index">1</sub><i>t</i><sub class="lower-index">2</sub>... <i>t</i><sub class="lower-index"><i>i</i> - 1</sub></span>, the second one will contain a string consisting of a single character <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, the third one contains string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> + 1</sub><i>t</i><sub class="lower-index"><i>i</i> + 2</sub>... <i>t</i><sub class="lower-index">|<i>t</i>|</sub></span>. </li></ol><center> <img class="tex-graphics" src="file://XqLPOuo5.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script">An example of making action <span class="tex-span">(<i>i</i> = 4)</span> with string <span class="tex-span"><i>s</i></span> = «<span class="tex-font-style-tt">abacaba</span>»</span> </center><p>Your task is to determine the winner provided that both players play optimally well. If the first player wins, find the position of character that is optimal to cut in his first move. If there are multiple positions, print the minimal possible one.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>). It is guaranteed that string <span class="tex-span"><i>s</i></span> only contains lowercase English letters.</p></div><div class="output-specification"><p>If the second player wins, print in the single line "<span class="tex-font-style-tt">Second</span>" (without the quotes). Otherwise, print in the first line "<span class="tex-font-style-tt">First</span>" (without the quotes), and in the second line print the minimal possible winning move — integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ |<i>s</i>|)</span>.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>). It is guaranteed that string <span class="tex-span"><i>s</i></span> only contains lowercase English letters.</p>

## Output

<p>If the second player wins, print in the single line "<span class="tex-font-style-tt">Second</span>" (without the quotes). Otherwise, print in the first line "<span class="tex-font-style-tt">First</span>" (without the quotes), and in the second line print the minimal possible winning move — integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ |<i>s</i>|)</span>.</p>





```input1
abacaba

```




```input2
abcde

```




```output1
First
2

```




```output2
Second

```



## Note

<p>In the first sample the first player has multiple winning moves. But the minimum one is to cut the character in position <span class="tex-span">2</span>. </p><p>In the second sample the first player has no available moves.</p>
