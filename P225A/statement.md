## Description

<div><p>A dice is a cube, its faces contain distinct integers from 1 to 6 as black points. The sum of numbers at the opposite dice faces always equals 7. Please note that there are only two dice (these dices are mirror of each other) that satisfy the given constraints (both of them are shown on the picture on the left).</p><center> <img class="tex-graphics" src="file://49Hq8vDI.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Alice and Bob play dice. Alice has built a tower from <span class="tex-span"><i>n</i></span> dice. We know that in this tower the adjacent dice contact with faces with distinct numbers. Bob wants to uniquely identify the numbers written on the faces of all dice, from which the tower is built. Unfortunately, Bob is looking at the tower from the face, and so he does not see all the numbers on the faces. Bob sees the number on the top of the tower and the numbers on the two adjacent sides (on the right side of the picture shown what Bob sees).</p><p>Help Bob, tell whether it is possible to uniquely identify the numbers on the faces of all the dice in the tower, or not.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of dice in the tower.</p><p>The second line contains an integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ 6)</span> — the number Bob sees at the top of the tower. Next <span class="tex-span"><i>n</i></span> lines contain two space-separated integers each: the <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 6;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the numbers Bob sees on the two sidelong faces of the <span class="tex-span"><i>i</i></span>-th dice in the tower.</p><p>Consider the dice in the tower indexed from top to bottom from 1 to <span class="tex-span"><i>n</i></span>. That is, the topmost dice has index 1 (the dice whose top face Bob can see). It is guaranteed that it is possible to make a dice tower that will look as described in the input.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if it is possible to to uniquely identify the numbers on the faces of all the dice in the tower. If it is impossible, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of dice in the tower.</p><p>The second line contains an integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ 6)</span> — the number Bob sees at the top of the tower. Next <span class="tex-span"><i>n</i></span> lines contain two space-separated integers each: the <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 6;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the numbers Bob sees on the two sidelong faces of the <span class="tex-span"><i>i</i></span>-th dice in the tower.</p><p>Consider the dice in the tower indexed from top to bottom from 1 to <span class="tex-span"><i>n</i></span>. That is, the topmost dice has index 1 (the dice whose top face Bob can see). It is guaranteed that it is possible to make a dice tower that will look as described in the input.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if it is possible to to uniquely identify the numbers on the faces of all the dice in the tower. If it is impossible, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
3
6
3 2
5 4
2 4

```




```input2
3
3
2 6
4 1
5 3

```




```output1
YES
```




```output2
NO
```


