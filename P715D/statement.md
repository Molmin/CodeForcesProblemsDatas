## Description

<div><p>ZS the Coder loves mazes. Your job is to create one so that he can play with it. A maze consists of <span class="tex-span"><i>n</i> × <i>m</i></span> rooms, and the rooms are arranged in <span class="tex-span"><i>n</i></span> rows (numbered from the top to the bottom starting from <span class="tex-span">1</span>) and <span class="tex-span"><i>m</i></span> columns (numbered from the left to the right starting from <span class="tex-span">1</span>). The room in the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column is denoted by <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. A player starts in the room <span class="tex-span">(1, 1)</span> and wants to reach the room <span class="tex-span">(<i>n</i>, <i>m</i>)</span>.</p><p>Each room has four doors (except for ones at the maze border), one on each of its walls, and two adjacent by the wall rooms shares the same door. Some of the doors are locked, which means it is impossible to pass through the door. For example, if the door connecting <span class="tex-span">(<i>i</i>, <i>j</i>)</span> and <span class="tex-span">(<i>i</i>, <i>j</i> + 1)</span> is locked, then we can't go from <span class="tex-span">(<i>i</i>, <i>j</i>)</span> to <span class="tex-span">(<i>i</i>, <i>j</i> + 1)</span>. Also, one can only travel between the rooms downwards (from the room <span class="tex-span">(<i>i</i>, <i>j</i>)</span> to the room <span class="tex-span">(<i>i</i> + 1, <i>j</i>)</span>) or rightwards (from the room <span class="tex-span">(<i>i</i>, <i>j</i>)</span> to the room <span class="tex-span">(<i>i</i>, <i>j</i> + 1)</span>) provided the corresponding door is not locked.</p><center> <img class="tex-graphics" src="file://AqYaM4dQ.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">This image represents a maze with some doors locked. The colored arrows denotes all the possible paths while a red cross denotes a locked door.</span> </center><p>ZS the Coder considers a maze to have <span class="tex-font-style-it">difficulty</span> <span class="tex-span"><i>x</i></span> if there is exactly <span class="tex-span"><i>x</i></span> ways of travelling from the room <span class="tex-span">(1, 1)</span> to the room <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. Two ways are considered different if they differ by the sequence of rooms visited while travelling.</p><p>Your task is to create a maze such that its difficulty is exactly equal to <span class="tex-span"><i>T</i></span>. In addition, ZS the Coder doesn't like large mazes, so the size of the maze and the number of locked doors are limited. Sounds simple enough, right?</p></div><div class="input-specification"><p>The first and only line of the input contains a single integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">18</sup></span>), the difficulty of the required maze.</p></div><div class="output-specification"><p>The first line should contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>)&nbsp;— the number of rows and columns of the maze respectively.</p><p>The next line should contain a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 300</span>)&nbsp;— the number of locked doors in the maze.</p><p>Then, <span class="tex-span"><i>k</i></span> lines describing locked doors should follow. Each of them should contain four integers, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>. This means that the door connecting room <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and room <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> is locked. Note that room <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> should be adjacent either to the right or to the bottom of <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, i.e. <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> + <i>y</i><sub class="lower-index">2</sub></span> should be equal to <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> + <i>y</i><sub class="lower-index">1</sub> + 1</span>. There should not be a locked door that appears twice in the list.</p><p>It is guaranteed that at least one solution exists. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first and only line of the input contains a single integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">18</sup></span>), the difficulty of the required maze.</p>

## Output

<p>The first line should contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>)&nbsp;— the number of rows and columns of the maze respectively.</p><p>The next line should contain a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 300</span>)&nbsp;— the number of locked doors in the maze.</p><p>Then, <span class="tex-span"><i>k</i></span> lines describing locked doors should follow. Each of them should contain four integers, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>. This means that the door connecting room <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and room <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> is locked. Note that room <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> should be adjacent either to the right or to the bottom of <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, i.e. <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> + <i>y</i><sub class="lower-index">2</sub></span> should be equal to <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> + <i>y</i><sub class="lower-index">1</sub> + 1</span>. There should not be a locked door that appears twice in the list.</p><p>It is guaranteed that at least one solution exists. If there are multiple solutions, print any of them.</p>





```input1
3

```




```input2
4

```




```output1
3 2
0

```




```output2
4 3
3
1 2 2 2
3 2 3 3
1 3 2 3
```



## Note

<p>Here are how the sample input and output looks like. The colored arrows denotes all the possible paths while a red cross denotes a locked door.</p><p>In the first sample case:</p><center> <img class="tex-graphics" src="file://cQLamIm6.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample case:</p><center> <img class="tex-graphics" src="file://0pEq0jlK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
