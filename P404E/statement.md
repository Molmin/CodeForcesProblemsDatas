## Description

<div><p>Valera has a strip infinite in both directions and consisting of cells. The cells are numbered by integers. The cell number <span class="tex-span">0</span> has a robot.</p><p>The robot has instructions — the sequence of moves that he must perform. In one move, the robot moves one cell to the left or one cell to the right, according to instructions. Before the robot starts moving, Valera puts obstacles in some cells of the strip, excluding cell number <span class="tex-span">0</span>. If the robot should go into the cell with an obstacle according the instructions, it will skip this move.</p><p>Also Valera indicates the finish cell in which the robot has to be after completing the entire instructions. The finishing cell should be different from the starting one. It is believed that the robot <span class="tex-font-style-it">completed the instructions successfully</span>, if during the process of moving he visited the finish cell exactly once — at its last move. Moreover, the latter move cannot be skipped.</p><p>Let's assume that <span class="tex-span"><i>k</i></span> is the minimum number of obstacles that Valera must put to make the robot able to complete the entire sequence of instructions successfully and end up in some finishing cell. You need to calculate in how many ways Valera can choose <span class="tex-span"><i>k</i></span> obstacles and the finishing cell so that the robot is able to complete the instructions successfully.</p></div><div class="input-specification"><p>The first line contains a sequence of characters without spaces <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>, consisting only of letters "<span class="tex-font-style-tt">L</span>" and "<span class="tex-font-style-tt">R</span>". If character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">L</span>", then the robot on the <span class="tex-span"><i>i</i></span>-th move must try to move one cell to the left. If the <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>-th character equals "<span class="tex-font-style-tt">R</span>", then the robot on the <span class="tex-span"><i>i</i></span>-th move must try to move one cell to the right.</p></div><div class="output-specification"><p>Print a single integer — the required number of ways. It's guaranteed that this number fits into 64-bit signed integer type.</p></div>

## Input

<p>The first line contains a sequence of characters without spaces <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>, consisting only of letters "<span class="tex-font-style-tt">L</span>" and "<span class="tex-font-style-tt">R</span>". If character <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">L</span>", then the robot on the <span class="tex-span"><i>i</i></span>-th move must try to move one cell to the left. If the <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>-th character equals "<span class="tex-font-style-tt">R</span>", then the robot on the <span class="tex-span"><i>i</i></span>-th move must try to move one cell to the right.</p>

## Output

<p>Print a single integer — the required number of ways. It's guaranteed that this number fits into 64-bit signed integer type.</p>





```input1
RR

```




```input2
RRL

```




```output1
1

```




```output2
1

```



## Note

<p>In the first sample Valera mustn't add any obstacles and his finishing cell must be cell <span class="tex-span">2</span>.</p><p>In the second sample, Valera must add an obstacle in cell number <span class="tex-span">1</span>, and his finishing cell must be cell number <span class="tex-span"> - 1</span>. In this case robot skips the first two moves and on the third move he goes straight from the starting cell to the finishing one. But if Valera doesn't add any obstacles, or adds an obstacle to another cell, then the robot visits the finishing cell more than once.</p>
