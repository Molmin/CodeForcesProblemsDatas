## Description

<div><p>You are at a water bowling training. There are <span class="tex-span"><i>l</i></span> people who play with their left hand, <span class="tex-span"><i>r</i></span> people, who play with their right hand, and <span class="tex-span"><i>a</i></span> ambidexters, who can play with left or right hand.</p><p>The coach decided to form a team of even number of players, exactly half of the players should play with their right hand, and exactly half of the players should play with their left hand. One player should use only on of his hands.</p><p>Ambidexters play as well with their right hand as with their left hand. In the team, an ambidexter can play with their left hand, or with their right hand.</p><p>Please find the maximum possible size of the team, where equal number of players use their left and right hands, respectively.</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 ≤ <i>l</i>, <i>r</i>, <i>a</i> ≤ 100</span>) — the number of left-handers, the number of right-handers and the number of ambidexters at the training. </p></div><div class="output-specification"><p>Print a single even integer&nbsp;— the maximum number of players in the team. It is possible that the team can only have zero number of players.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 ≤ <i>l</i>, <i>r</i>, <i>a</i> ≤ 100</span>) — the number of left-handers, the number of right-handers and the number of ambidexters at the training. </p>

## Output

<p>Print a single even integer&nbsp;— the maximum number of players in the team. It is possible that the team can only have zero number of players.</p>





```input1
1 4 2

```




```input2
5 5 5

```




```input3
0 2 0

```




```output1
6

```




```output2
14

```




```output3
0

```



## Note

<p>In the first example you can form a team of <span class="tex-span">6</span> players. You should take the only left-hander and two ambidexters to play with left hand, and three right-handers to play with right hand. The only person left can't be taken into the team.</p><p>In the second example you can form a team of <span class="tex-span">14</span> people. You have to take all five left-handers, all five right-handers, two ambidexters to play with left hand and two ambidexters to play with right hand.</p>
