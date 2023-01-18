## Description

<div><p>Theater stage is a rectangular field of size <span class="tex-span"><i>n</i> × <i>m</i></span>. The director gave you the stage's plan which actors will follow. For each cell it is stated in the plan if there would be an actor in this cell or not.</p><p>You are to place a spotlight on the stage in some <span class="tex-font-style-it">good</span> position. The spotlight will project light in one of the four directions (if you look at the stage from above)&nbsp;— left, right, up or down. Thus, the spotlight's position is a cell it is placed to and a direction it shines.</p><p>A position is <span class="tex-font-style-it">good</span> if two conditions hold: </p><ul> <li> there is no actor in the cell the spotlight is placed to; </li><li> there is at least one actor in the direction the spotlight projects. </li></ul><p>Count the number of <span class="tex-font-style-it">good</span> positions for placing the spotlight. Two positions of spotlight are considered to be different if the location cells or projection direction differ.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and the number of columns in the plan.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> integers, <span class="tex-span">0</span> or <span class="tex-span">1</span> each&nbsp;— the description of the plan. Integer <span class="tex-span">1</span>, means there will be an actor in the corresponding cell, while <span class="tex-span">0</span> means the cell will remain empty. It is guaranteed that there is at least one actor in the plan.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of <span class="tex-font-style-it">good</span> positions for placing the spotlight.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and the number of columns in the plan.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> integers, <span class="tex-span">0</span> or <span class="tex-span">1</span> each&nbsp;— the description of the plan. Integer <span class="tex-span">1</span>, means there will be an actor in the corresponding cell, while <span class="tex-span">0</span> means the cell will remain empty. It is guaranteed that there is at least one actor in the plan.</p>

## Output

<p>Print one integer&nbsp;— the number of <span class="tex-font-style-it">good</span> positions for placing the spotlight.</p>





```input1
2 4
0 1 0 0
1 0 1 0

```




```input2
4 4
0 0 0 0
1 0 0 1
0 1 1 0
0 1 0 0

```




```output1
9

```




```output2
20

```



## Note

<p>In the first example the following positions are <span class="tex-font-style-it">good</span>:</p><ol> <li> the (1, 1) cell and right direction; </li><li> the (1, 1) cell and down direction; </li><li> the (1, 3) cell and left direction; </li><li> the (1, 3) cell and down direction; </li><li> the (1, 4) cell and left direction; </li><li> the (2, 2) cell and left direction; </li><li> the (2, 2) cell and up direction; </li><li> the (2, 2) and right direction; </li><li> the (2, 4) cell and left direction. </li></ol><p>Therefore, there are <span class="tex-span">9</span> <span class="tex-font-style-it">good</span> positions in this example.</p>
