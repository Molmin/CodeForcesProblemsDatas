## Description

<div><p>During the loading of the game "Dungeons and Candies" you are required to get descriptions of <span class="tex-span"><i>k</i></span> levels from the server. Each description is a map of an <span class="tex-span"><i>n</i> × <i>m</i></span> checkered rectangular field. Some cells of the field contain candies (each cell has at most one candy). An empty cell is denoted as "<span class="tex-font-style-tt">.</span>" on the map, but if a cell has a candy, it is denoted as a letter of the English alphabet. A level may contain identical candies, in this case the letters in the corresponding cells of the map will be the same.</p><center> <img class="tex-graphics" src="file://Wxz6jL7U.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>When you transmit information via a network, you want to minimize traffic — the total size of the transferred data. The levels can be transmitted in any order. There are two ways to transmit the current level <span class="tex-span"><i>A</i></span>:</p><ol> <li> You can transmit the whole level <span class="tex-span"><i>A</i></span>. Then you need to transmit <span class="tex-span"><i>n</i>·<i>m</i></span> bytes via the network. </li><li> You can transmit the difference between level <span class="tex-span"><i>A</i></span> and some previously transmitted level <span class="tex-span"><i>B</i></span> (if it exists); this operation requires to transmit <span class="tex-span"><i>d</i><sub class="lower-index"><i>A</i>, <i>B</i></sub>·<i>w</i></span> bytes, where <span class="tex-span"><i>d</i><sub class="lower-index"><i>A</i>, <i>B</i></sub></span> is the number of cells of the field that are different for <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>, and <span class="tex-span"><i>w</i></span> is a constant. Note, that you should compare only the corresponding cells of levels <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> to calculate <span class="tex-span"><i>d</i><sub class="lower-index"><i>A</i>, <i>B</i></sub></span>. You cannot transform the maps of levels, i.e. rotate or shift them relatively to each other. </li></ol><p>Your task is to find a way to transfer all the <span class="tex-span"><i>k</i></span> levels and minimize the traffic.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>, <i>w</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10;&nbsp;1 ≤ <i>k</i>, <i>w</i> ≤ 1000)</span>. Then follows the description of <span class="tex-span"><i>k</i></span> levels. Each level is described by <span class="tex-span"><i>n</i></span> lines, each line contains <span class="tex-span"><i>m</i></span> characters. Each character is either a letter of the English alphabet or a dot ("<span class="tex-font-style-tt">.</span>"). Please note that the case of the letters matters.</p></div><div class="output-specification"><p>In the first line print the required minimum number of transferred bytes.</p><p>Then print <span class="tex-span"><i>k</i></span> pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub></span>, describing the way to transfer levels. Pair <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> means that level <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> needs to be transferred by way <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> equals 0, that means that the level must be transferred using the first way, otherwise <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> must be equal to the number of a previously transferred level. It means that you will transfer the difference between levels <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to transfer level <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Print the pairs in the order of transferring levels. The levels are numbered 1 through <span class="tex-span"><i>k</i></span> in the order they follow in the input.</p><p>If there are multiple optimal solutions, you can print any of them.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>, <i>w</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10;&nbsp;1 ≤ <i>k</i>, <i>w</i> ≤ 1000)</span>. Then follows the description of <span class="tex-span"><i>k</i></span> levels. Each level is described by <span class="tex-span"><i>n</i></span> lines, each line contains <span class="tex-span"><i>m</i></span> characters. Each character is either a letter of the English alphabet or a dot ("<span class="tex-font-style-tt">.</span>"). Please note that the case of the letters matters.</p>

## Output

<p>In the first line print the required minimum number of transferred bytes.</p><p>Then print <span class="tex-span"><i>k</i></span> pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub></span>, describing the way to transfer levels. Pair <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> means that level <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> needs to be transferred by way <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> equals 0, that means that the level must be transferred using the first way, otherwise <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> must be equal to the number of a previously transferred level. It means that you will transfer the difference between levels <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to transfer level <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Print the pairs in the order of transferring levels. The levels are numbered 1 through <span class="tex-span"><i>k</i></span> in the order they follow in the input.</p><p>If there are multiple optimal solutions, you can print any of them.</p>





```input1
2 3 3 2
A.A
...
A.a
..C
X.Y
...

```




```input2
1 1 4 1
A
.
B
.

```




```input3
1 3 5 2
ABA
BBB
BBA
BAB
ABB

```




```output1
14
1 0
2 1
3 1

```




```output2
3
1 0
2 0
4 2
3 0

```




```output3
11
1 0
3 1
2 3
4 2
5 1

```


