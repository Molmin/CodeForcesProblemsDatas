## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cows playing poker at a table. For the current betting phase, each player's status is either "<span class="tex-font-style-tt">ALLIN</span>", "<span class="tex-font-style-tt">IN</span>", or "<span class="tex-font-style-tt">FOLDED</span>", and does not change throughout the phase. To increase the suspense, a player whose current status is not "<span class="tex-font-style-tt">FOLDED</span>" may show his/her hand to the table. However, so as not to affect any betting decisions, he/she may only do so if all other players have a status of either "<span class="tex-font-style-tt">ALLIN</span>" or "<span class="tex-font-style-tt">FOLDED</span>". The player's own status may be either "<span class="tex-font-style-tt">ALLIN</span>" or "<span class="tex-font-style-tt">IN</span>".</p><p>Find the number of cows that can currently show their hands without affecting any betting decisions.</p></div><div class="input-specification"><p>The first line contains a single integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> characters, each either "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">I</span>", or "<span class="tex-font-style-tt">F</span>". The <span class="tex-span"><i>i</i></span>-th character is "<span class="tex-font-style-tt">A</span>" if the <span class="tex-span"><i>i</i></span>-th player's status is "<span class="tex-font-style-tt">ALLIN</span>", "<span class="tex-font-style-tt">I</span>" if the <span class="tex-span"><i>i</i></span>-th player's status is "<span class="tex-font-style-tt">IN</span>", or "<span class="tex-font-style-tt">F</span>" if the <span class="tex-span"><i>i</i></span>-th player's status is "<span class="tex-font-style-tt">FOLDED</span>".</p></div><div class="output-specification"><p>The first line should contain a single integer denoting the number of players that can currently show their hands.</p></div>

## Input

<p>The first line contains a single integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> characters, each either "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">I</span>", or "<span class="tex-font-style-tt">F</span>". The <span class="tex-span"><i>i</i></span>-th character is "<span class="tex-font-style-tt">A</span>" if the <span class="tex-span"><i>i</i></span>-th player's status is "<span class="tex-font-style-tt">ALLIN</span>", "<span class="tex-font-style-tt">I</span>" if the <span class="tex-span"><i>i</i></span>-th player's status is "<span class="tex-font-style-tt">IN</span>", or "<span class="tex-font-style-tt">F</span>" if the <span class="tex-span"><i>i</i></span>-th player's status is "<span class="tex-font-style-tt">FOLDED</span>".</p>

## Output

<p>The first line should contain a single integer denoting the number of players that can currently show their hands.</p>





```input1
6
AFFAAA

```




```input2
3
AFI

```




```output1
4

```




```output2
1

```



## Note

<p>In the first sample, cows 1, 4, 5, and 6 can show their hands. In the second sample, only cow 3 can show her hand.</p>
