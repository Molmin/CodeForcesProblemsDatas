## Description

<div><p>The King of Flatland will organize a knights' tournament! The winner will get half the kingdom and the favor of the princess of legendary beauty and wisdom. The final test of the applicants' courage and strength will be a fencing tournament. The tournament is held by the following rules: the participants fight one on one, the winner (or rather, the survivor) transfers to the next round.</p><p>Before the battle both participants stand at the specified points on the <span class="tex-span"><i>Ox</i></span> axis with integer coordinates. Then they make moves in turn. The first participant moves first, naturally. During a move, the first participant can transfer from the point <span class="tex-span"><i>x</i></span> to any integer point of the interval [<span class="tex-span"><i>x</i> + <i>a</i></span>; <span class="tex-span"><i>x</i> + <i>b</i></span>]. The second participant can transfer during a move to any integer point of the interval [<span class="tex-span"><i>x</i> - <i>b</i></span>; <span class="tex-span"><i>x</i> - <i>a</i></span>]. That is, the options for the players' moves are symmetric (note that the numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are not required to be positive, and if <span class="tex-span"><i>a</i> ≤ 0 ≤ <i>b</i></span>, then staying in one place is a correct move). At any time the participants can be located arbitrarily relative to each other, that is, it is allowed to "jump" over the enemy in any direction. A participant wins if he uses his move to transfer to the point where his opponent is.</p><p>Of course, the princess has already chosen a husband and now she wants to make her sweetheart win the tournament. He has already reached the tournament finals and he is facing the last battle. The princess asks the tournament manager to arrange the tournament finalists in such a way that her sweetheart wins the tournament, considering that both players play optimally. However, the initial location of the participants has already been announced, and we can only pull some strings and determine which participant will be first and which one will be second. But how do we know which participant can secure the victory? Alas, the princess is not learned in the military affairs... Therefore, she asks you to determine how the battle will end considering that both opponents play optimally. Also, if the first player wins, your task is to determine his winning move.</p></div><div class="input-specification"><p>The first line contains four space-separated integers — <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≠ <i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i> ≤ <i>b</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>) — coordinates of the points where the first and the second participant start, and the numbers that determine the players' moves, correspondingly.</p></div><div class="output-specification"><p>On the first line print the outcome of the battle as "<span class="tex-font-style-tt">FIRST</span>" (without the quotes), if both players play optimally and the first player wins. Print "<span class="tex-font-style-tt">SECOND</span>" (without the quotes) if the second player wins and print "<span class="tex-font-style-tt">DRAW</span>" (without the quotes), if nobody is able to secure the victory.</p><p>If the first player wins, print on the next line the single integer <span class="tex-span"><i>x</i></span> — the coordinate of the point where the first player should transfer to win. The indicated move should be valid, that is, it should meet the following condition: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> + <i>a</i> ≤ <i>x</i> ≤ <i>x</i><sub class="lower-index">1</sub> + <i>b</i></span>. If there are several winning moves, print any of them. If the first participant can't secure the victory, then you do not have to print anything.</p></div>

## Input

<p>The first line contains four space-separated integers — <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≠ <i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i> ≤ <i>b</i></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>) — coordinates of the points where the first and the second participant start, and the numbers that determine the players' moves, correspondingly.</p>

## Output

<p>On the first line print the outcome of the battle as "<span class="tex-font-style-tt">FIRST</span>" (without the quotes), if both players play optimally and the first player wins. Print "<span class="tex-font-style-tt">SECOND</span>" (without the quotes) if the second player wins and print "<span class="tex-font-style-tt">DRAW</span>" (without the quotes), if nobody is able to secure the victory.</p><p>If the first player wins, print on the next line the single integer <span class="tex-span"><i>x</i></span> — the coordinate of the point where the first player should transfer to win. The indicated move should be valid, that is, it should meet the following condition: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> + <i>a</i> ≤ <i>x</i> ≤ <i>x</i><sub class="lower-index">1</sub> + <i>b</i></span>. If there are several winning moves, print any of them. If the first participant can't secure the victory, then you do not have to print anything.</p>





```input1
0 2 0 4

```




```input2
0 2 1 1

```




```input3
0 2 0 1

```




```output1
FIRST
2

```




```output2
SECOND

```




```output3
DRAW

```



## Note

<p>In the first sample the first player can win in one move.</p><p>In the second sample the first participant must go to point <span class="tex-span">1</span>, where the second participant immediately goes and wins. </p><p>In the third sample changing the position isn't profitable to either participant, so nobody wins.</p>
