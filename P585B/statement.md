## Description

<div><p>The mobile application store has a new game called "Subway Roller".</p><p>The protagonist of the game Philip is located in one end of the tunnel and wants to get out of the other one. The tunnel is a rectangular field consisting of three rows and <span class="tex-span"><i>n</i></span> columns. At the beginning of the game the hero is in some cell of the leftmost column. Some number of trains rides towards the hero. Each train consists of two or more neighbouring cells in some row of the field.</p><p>All trains are moving from right to left at a speed of two cells per second, and the hero runs from left to right at the speed of one cell per second. For simplicity, the game is implemented so that the hero and the trains move in turns. First, the hero moves one cell to the right, then one square up or down, or stays idle. Then all the trains move twice simultaneously one cell to the left. Thus, in one move, Philip definitely makes a move to the right and can move up or down. If at any point, Philip is in the same cell with a train, he loses. If the train reaches the left column, it continues to move as before, leaving the tunnel.</p><p>Your task is to answer the question whether there is a sequence of movements of Philip, such that he would be able to get to the rightmost column.</p><center> <img class="tex-graphics" src="file://pnZjvC2W.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>Each test contains from one to ten sets of the input data. The first line of the test contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10</span> for pretests and tests or <span class="tex-span"><i>t</i> = 1</span> for hacks; see the Notes section for details) — the number of sets.</p><p>Then follows the description of <span class="tex-span"><i>t</i></span> sets of the input data. </p><p>The first line of the description of each set contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100, 1 ≤ <i>k</i> ≤ 26</span>) — the number of columns on the field and the number of trains. Each of the following three lines contains the sequence of <span class="tex-span"><i>n</i></span> character, representing the row of the field where the game is on. Philip's initial position is marked as '<span class="tex-font-style-tt">s</span>', he is in the leftmost column. Each of the <span class="tex-span"><i>k</i></span> trains is marked by some sequence of identical uppercase letters of the English alphabet, located in one line. Distinct trains are represented by distinct letters. Character '<span class="tex-font-style-tt">.</span>' represents an empty cell, that is, the cell that doesn't contain either Philip or the trains.</p></div><div class="output-specification"><p>For each set of the input data print on a single line word <span class="tex-font-style-tt">YES</span>, if it is possible to win the game and word <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>Each test contains from one to ten sets of the input data. The first line of the test contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10</span> for pretests and tests or <span class="tex-span"><i>t</i> = 1</span> for hacks; see the Notes section for details) — the number of sets.</p><p>Then follows the description of <span class="tex-span"><i>t</i></span> sets of the input data. </p><p>The first line of the description of each set contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100, 1 ≤ <i>k</i> ≤ 26</span>) — the number of columns on the field and the number of trains. Each of the following three lines contains the sequence of <span class="tex-span"><i>n</i></span> character, representing the row of the field where the game is on. Philip's initial position is marked as '<span class="tex-font-style-tt">s</span>', he is in the leftmost column. Each of the <span class="tex-span"><i>k</i></span> trains is marked by some sequence of identical uppercase letters of the English alphabet, located in one line. Distinct trains are represented by distinct letters. Character '<span class="tex-font-style-tt">.</span>' represents an empty cell, that is, the cell that doesn't contain either Philip or the trains.</p>

## Output

<p>For each set of the input data print on a single line word <span class="tex-font-style-tt">YES</span>, if it is possible to win the game and word <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
2
16 4
...AAAAA........
s.BBB......CCCCC
........DDDDD...
16 4
...AAAAA........
s.BBB....CCCCC..
.......DDDDD....

```




```input2
2
10 4
s.ZZ......
.....AAABB
.YYYYYY...
10 4
s.ZZ......
....AAAABB
.YYYYYY...

```




```output1
YES
NO

```




```output2
YES
NO

```



## Note

<p>In the first set of the input of the first sample Philip must first go forward and go down to the third row of the field, then go only forward, then go forward and climb to the second row, go forward again and go up to the first row. After that way no train blocks Philip's path, so he can go straight to the end of the tunnel.</p><p>Note that in this problem the challenges are restricted to tests that contain only one testset.</p>
