## Description

<div><p>Two boys decided to compete in text typing on the site "Key races". During the competition, they have to type a text consisting of <span class="tex-span"><i>s</i></span> characters. The first participant types one character in <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> milliseconds and has ping <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> milliseconds. The second participant types one character in <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> milliseconds and has ping <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> milliseconds.</p><p>If connection ping (delay) is <span class="tex-span"><i>t</i></span> milliseconds, the competition passes for a participant as follows: </p><ol> <li> Exactly after <span class="tex-span"><i>t</i></span> milliseconds after the start of the competition the participant receives the text to be entered. </li><li> Right after that he starts to type it. </li><li> Exactly <span class="tex-span"><i>t</i></span> milliseconds after he ends typing all the text, the site receives information about it. </li></ol><p>The winner is the participant whose information on the success comes earlier. If the information comes from both participants at the same time, it is considered that there is a draw.</p><p>Given the length of the text and the information about participants, determine the result of the game.</p></div><div class="input-specification"><p>The first line contains five integers <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub> ≤ 1000</span>)&nbsp;— the number of characters in the text, the time of typing one character for the first participant, the time of typing one character for the the second participant, the ping of the first participant and the ping of the second participant.</p></div><div class="output-specification"><p>If the first participant wins, print "<span class="tex-font-style-tt">First</span>". If the second participant wins, print "<span class="tex-font-style-tt">Second</span>". In case of a draw print "<span class="tex-font-style-tt">Friendship</span>".</p></div>

## Input

<p>The first line contains five integers <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub> ≤ 1000</span>)&nbsp;— the number of characters in the text, the time of typing one character for the first participant, the time of typing one character for the the second participant, the ping of the first participant and the ping of the second participant.</p>

## Output

<p>If the first participant wins, print "<span class="tex-font-style-tt">First</span>". If the second participant wins, print "<span class="tex-font-style-tt">Second</span>". In case of a draw print "<span class="tex-font-style-tt">Friendship</span>".</p>





```input1
5 1 2 1 2

```




```input2
3 3 1 1 1

```




```input3
4 5 3 1 5

```




```output1
First

```




```output2
Second

```




```output3
Friendship

```



## Note

<p>In the first example, information on the success of the first participant comes in <span class="tex-span">7</span> milliseconds, of the second participant&nbsp;— in <span class="tex-span">14</span> milliseconds. So, the first wins.</p><p>In the second example, information on the success of the first participant comes in <span class="tex-span">11</span> milliseconds, of the second participant&nbsp;— in <span class="tex-span">5</span> milliseconds. So, the second wins.</p><p>In the third example, information on the success of the first participant comes in <span class="tex-span">22</span> milliseconds, of the second participant&nbsp;— in <span class="tex-span">22</span> milliseconds. So, it is be a draw.</p>
