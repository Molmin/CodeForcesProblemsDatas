## Description

<div><p>Om Nom really likes candies and doesn't like spiders as they frequently steal candies. One day Om Nom fancied a walk in a park. Unfortunately, the park has some spiders and Om Nom doesn't want to see them at all.</p><center> <img class="tex-graphics" src="file://nPmTVqYR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The park can be represented as a rectangular <span class="tex-span"><i>n</i> × <i>m</i></span> field. The park has <span class="tex-span"><i>k</i></span> spiders, each spider at time 0 is at some cell of the field. The spiders move all the time, and each spider always moves in one of the four directions (left, right, down, up). In a unit of time, a spider crawls from his cell to the side-adjacent cell in the corresponding direction. If there is no cell in the given direction, then the spider leaves the park. The spiders do not interfere with each other as they move. Specifically, one cell can have multiple spiders at the same time.</p><p>Om Nom isn't yet sure where to start his walk from but he definitely wants:</p><ul> <li> to start walking at time 0 at an upper row cell of the field (it is guaranteed that the cells in this row do not contain any spiders); </li><li> to walk by moving down the field towards the lowest row (the walk ends when Om Nom leaves the boundaries of the park). </li></ul><p>We know that Om Nom moves by jumping. One jump takes one time unit and transports the little monster from his cell to either a side-adjacent cell on the lower row or outside the park boundaries.</p><p>Each time Om Nom lands in a cell he sees all the spiders that have come to that cell at this moment of time. Om Nom wants to choose the optimal cell to start the walk from. That's why he wonders: for each possible starting cell, how many spiders will he see during the walk if he starts from this cell? Help him and calculate the required value for each possible starting cell.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 2000;&nbsp;0 ≤ <i>k</i> ≤ <i>m</i>(<i>n</i> - 1))</span>. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the park. The characters in the <span class="tex-span"><i>i</i></span>-th line describe the <span class="tex-span"><i>i</i></span>-th row of the park field. If the character in the line equals "<span class="tex-font-style-tt">.</span>", that means that the corresponding cell of the field is empty; otherwise, the character in the line will equal one of the four characters: "<span class="tex-font-style-tt">L</span>" (meaning that this cell has a spider at time 0, moving left), "<span class="tex-font-style-tt">R</span>" (a spider moving right), "<span class="tex-font-style-tt">U</span>" (a spider moving up), "<span class="tex-font-style-tt">D</span>" (a spider moving down). </p><p>It is guaranteed that the first row doesn't contain any spiders. It is guaranteed that the description of the field contains no extra characters. It is guaranteed that at time 0 the field contains exactly <span class="tex-span"><i>k</i></span> spiders.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers: the <span class="tex-span"><i>j</i></span>-th integer must show the number of spiders Om Nom will see if he starts his walk from the <span class="tex-span"><i>j</i></span>-th cell of the first row. The cells in any row of the field are numbered from left to right.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 2000;&nbsp;0 ≤ <i>k</i> ≤ <i>m</i>(<i>n</i> - 1))</span>. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the park. The characters in the <span class="tex-span"><i>i</i></span>-th line describe the <span class="tex-span"><i>i</i></span>-th row of the park field. If the character in the line equals "<span class="tex-font-style-tt">.</span>", that means that the corresponding cell of the field is empty; otherwise, the character in the line will equal one of the four characters: "<span class="tex-font-style-tt">L</span>" (meaning that this cell has a spider at time 0, moving left), "<span class="tex-font-style-tt">R</span>" (a spider moving right), "<span class="tex-font-style-tt">U</span>" (a spider moving up), "<span class="tex-font-style-tt">D</span>" (a spider moving down). </p><p>It is guaranteed that the first row doesn't contain any spiders. It is guaranteed that the description of the field contains no extra characters. It is guaranteed that at time 0 the field contains exactly <span class="tex-span"><i>k</i></span> spiders.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers: the <span class="tex-span"><i>j</i></span>-th integer must show the number of spiders Om Nom will see if he starts his walk from the <span class="tex-span"><i>j</i></span>-th cell of the first row. The cells in any row of the field are numbered from left to right.</p>





```input1
3 3 4
...
R.L
R.U

```




```input2
2 2 2
..
RL

```




```input3
2 2 2
..
LR

```




```input4
3 4 8
....
RRLL
UUUU

```




```input5
2 2 2
..
UU

```




```output1
0 2 2
```




```output2
1 1
```




```output3
0 0
```




```output4
1 3 3 1
```




```output5
0 0
```



## Note

<p>Consider the first sample. The notes below show how the spider arrangement changes on the field over time:</p><pre class="verbatim"><br>...        ...        ..U       ...<br>R.L   -&gt;   .*U   -&gt;   L.R   -&gt;  ...<br>R.U        .R.        ..R       ...<br><br></pre><p>Character "<span class="tex-font-style-tt">*</span>" represents a cell that contains two spiders at the same time.</p><ul> <li> If Om Nom starts from the first cell of the first row, he won't see any spiders. </li><li> If he starts from the second cell, he will see two spiders at time 1. </li><li> If he starts from the third cell, he will see two spiders: one at time 1, the other one at time 2. </li></ul>
