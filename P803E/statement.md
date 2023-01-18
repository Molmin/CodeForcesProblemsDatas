## Description

<div><p>Each evening Roma plays online poker on his favourite website. The rules of poker on this website are a bit strange: there are always two players in a hand, there are no bets, and the winner takes <span class="tex-span">1</span> virtual bourle from the loser.</p><p>Last evening Roma started to play poker. He decided to spend no more than <span class="tex-span"><i>k</i></span> virtual bourles — he will stop immediately if the number of his loses exceeds the number of his wins by <span class="tex-span"><i>k</i></span>. Also Roma will leave the game if he wins enough money for the evening, i.e. if the number of wins exceeds the number of loses by <span class="tex-span"><i>k</i></span>.</p><p>Next morning Roma found a piece of paper with a sequence on it representing his results. Roma doesn't remember the results exactly, and some characters in the sequence are written in a way such that it's impossible to recognize this character, so Roma can't recall whether he won <span class="tex-span"><i>k</i></span> bourles or he lost.</p><p>The sequence written by Roma is a string <span class="tex-span"><i>s</i></span> consisting of characters <span class="tex-font-style-tt">W</span> (Roma won the corresponding hand), <span class="tex-font-style-tt">L</span> (Roma lost), <span class="tex-font-style-tt">D</span> (draw) and <span class="tex-font-style-tt">?</span> (unknown result). Roma wants to restore any <span class="tex-font-style-it">valid</span> sequence by changing all <span class="tex-font-style-tt">?</span> characters to <span class="tex-font-style-tt">W</span>, <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">D</span>. The sequence is called <span class="tex-font-style-it">valid</span> if all these conditions are met: </p><ul> <li> In the end the absolute difference between the number of wins and loses is equal to <span class="tex-span"><i>k</i></span>; </li><li> There is no hand such that the absolute difference before this hand was equal to <span class="tex-span"><i>k</i></span>. </li></ul><p>Help Roma to restore any such sequence.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> (the length of Roma's sequence) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000</span>).</p><p>The second line contains the sequence <span class="tex-span"><i>s</i></span> consisting of characters <span class="tex-font-style-tt">W</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">D</span> and <span class="tex-font-style-tt">?</span>. There are exactly <span class="tex-span"><i>n</i></span> characters in this sequence.</p></div><div class="output-specification"><p>If there is no <span class="tex-font-style-it">valid</span> sequence that can be obtained from <span class="tex-span"><i>s</i></span> by replacing all <span class="tex-font-style-tt">?</span> characters by <span class="tex-font-style-tt">W</span>, <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">D</span>, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise print this sequence. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> (the length of Roma's sequence) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000</span>).</p><p>The second line contains the sequence <span class="tex-span"><i>s</i></span> consisting of characters <span class="tex-font-style-tt">W</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">D</span> and <span class="tex-font-style-tt">?</span>. There are exactly <span class="tex-span"><i>n</i></span> characters in this sequence.</p>

## Output

<p>If there is no <span class="tex-font-style-it">valid</span> sequence that can be obtained from <span class="tex-span"><i>s</i></span> by replacing all <span class="tex-font-style-tt">?</span> characters by <span class="tex-font-style-tt">W</span>, <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">D</span>, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise print this sequence. If there are multiple answers, print any of them.</p>





```input1
3 2
L??

```




```input2
3 1
W??

```




```input3
20 5
?LLLLLWWWWW?????????

```




```output1
LDL

```




```output2
NO

```




```output3
WLLLLLWWWWWWWWLWLWDW

```


