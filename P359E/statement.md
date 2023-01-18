## Description

<div><p>Simon loves neatness. So before he goes to bed, Simon wants to complete all chores in the house.</p><p>Simon's house looks like a rectangular table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns from above. All rows of the table are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom. All columns of the table are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Each cell of the table is a room. Pair <span class="tex-span">(<i>x</i>, <i>y</i>)</span> denotes the room, located at the intersection of the <span class="tex-span"><i>x</i></span>-th row and the <span class="tex-span"><i>y</i></span>-th column. For each room we know if the light is on or not there.</p><p>Initially Simon is in room <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>)</span>. He wants to turn off the lights in all the rooms in the house, and then return to room <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>)</span>. Suppose that at the current moment Simon is in the room <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. To reach the desired result, he can perform the following steps:</p><ol> <li> The format of the action is "<span class="tex-font-style-tt">1</span>". The action is to turn on the light in room <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Simon cannot do it if the room already has light on. </li><li> The format of the action is "<span class="tex-font-style-tt">2</span>". The action is to turn off the light in room <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Simon cannot do it if the room already has light off. </li><li> The format of the action is "<span class="tex-font-style-tt">dir</span>" (<span class="tex-span"><i>dir</i></span> is a character). The action is to move to a side-adjacent room in direction <span class="tex-span"><i>dir</i></span>. The direction can be left, right, up or down (the corresponding dir is <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">U</span> or <span class="tex-font-style-tt">D</span>). Additionally, Simon can move only if he see a light in the direction <span class="tex-span"><i>dir</i></span>. More formally, if we represent the room, Simon wants to go, as <span class="tex-span">(<i>nx</i>, <i>ny</i>)</span>, there shold be an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &gt; 0)</span>, that room <span class="tex-span">(<i>x</i> + (<i>nx</i> - <i>x</i>)<i>k</i>, <i>y</i> + (<i>ny</i> - <i>y</i>)<i>k</i>)</span> has a light. Of course, Simon cannot move out of his house. </li></ol><p>Help Simon, find the sequence of actions that lets him achieve the desired result.</p></div><div class="input-specification"><p>The first line contains three positive integers <span class="tex-span"><i>n</i>, <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 500, 1 ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub> ≤ <i>n</i>)</span>.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of rooms in the house. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>in</i></sub></span>. If number <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals zero, then room <span class="tex-span">(<i>i</i>, <i>j</i>)</span> has light off, and if number <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals one, then room <span class="tex-span">(<i>i</i>, <i>j</i>)</span> has light on. It is guaranteed that at least one room has light on.</p></div><div class="output-specification"><p>If there is no desired sequence of actions, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without the quotes) and the description of the required sequence of actions as a string. Note that you do not have to minimize the length of the sequence of actions but you shouldn't use more than <span class="tex-span">3·10<sup class="upper-index">6</sup></span> actions.</p></div>

## Input

<p>The first line contains three positive integers <span class="tex-span"><i>n</i>, <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 500, 1 ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub> ≤ <i>n</i>)</span>.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of rooms in the house. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>in</i></sub></span>. If number <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals zero, then room <span class="tex-span">(<i>i</i>, <i>j</i>)</span> has light off, and if number <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals one, then room <span class="tex-span">(<i>i</i>, <i>j</i>)</span> has light on. It is guaranteed that at least one room has light on.</p>

## Output

<p>If there is no desired sequence of actions, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without the quotes) and the description of the required sequence of actions as a string. Note that you do not have to minimize the length of the sequence of actions but you shouldn't use more than <span class="tex-span">3·10<sup class="upper-index">6</sup></span> actions.</p>





```input1
3 1 1
1 0 0
0 1 0
1 0 0

```




```input2
3 1 1
1 0 0
0 1 0
0 0 1

```




```output1
YES
D1R2L2D2UU2

```




```output2
NO

```


