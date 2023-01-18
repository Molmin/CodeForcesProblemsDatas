## Description

<div><p>Inna loves sweets very much. That's why she decided to play a game called "Sweet Matrix".</p><p>Inna sees an <span class="tex-span"><i>n</i> × <i>m</i></span> matrix and <span class="tex-span"><i>k</i></span> candies. We'll index the matrix rows from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the matrix columns from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. We'll represent the cell in the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column as <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. Two cells <span class="tex-span">(<i>i</i>, <i>j</i>)</span> and <span class="tex-span">(<i>p</i>, <i>q</i>)</span> of the matrix are <span class="tex-font-style-it">adjacent</span> if <span class="tex-span">|<i>i</i> - <i>p</i>| + |<i>j</i> - <i>q</i>| = 1</span>. A <span class="tex-font-style-it">path</span> is a sequence of the matrix cells where each pair of neighbouring cells in the sequence is adjacent. We'll call the number of cells in the sequence the path's length.</p><p>Each cell of the matrix can have at most one candy. Initiallly, all the cells are empty. Inna is trying to place each of the <span class="tex-span"><i>k</i></span> candies in the matrix one by one. For each candy Inna chooses cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> that will contains the candy, and also chooses the path that starts in cell <span class="tex-span">(1, 1)</span> and ends in cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> and doesn't contain any candies. After that Inna moves the candy along the path from cell <span class="tex-span">(1, 1)</span> to cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, where the candy stays forever. If at some moment Inna can't choose a path for the candy, she loses. If Inna can place all the candies in the matrix in the described manner, then her penalty equals the sum of lengths of all the paths she has used.</p><p>Help Inna to minimize the penalty in the game.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 50, 1 ≤ <i>k</i> ≤ <i>n</i>·<i>m</i>)</span>.</p></div><div class="output-specification"><p>In the first line print an integer — Inna's minimum penalty in the game.</p><p>In the next <span class="tex-span"><i>k</i></span> lines print the description of the path for each candy. The description of the path of the candy that is placed <span class="tex-span"><i>i</i></span>-th should follow on the <span class="tex-span"><i>i</i></span>-th line. The description of a path is a sequence of cells. Each cell must be written in the format <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, where <span class="tex-span"><i>i</i></span> is the number of the row and <span class="tex-span"><i>j</i></span> is the number of the column. You are allowed to print extra whitespaces in the line. If there are multiple optimal solutions, print any of them.</p><p>Please follow the output format strictly! If your program passes the first pretest, then the output format is correct.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 50, 1 ≤ <i>k</i> ≤ <i>n</i>·<i>m</i>)</span>.</p>

## Output

<p>In the first line print an integer — Inna's minimum penalty in the game.</p><p>In the next <span class="tex-span"><i>k</i></span> lines print the description of the path for each candy. The description of the path of the candy that is placed <span class="tex-span"><i>i</i></span>-th should follow on the <span class="tex-span"><i>i</i></span>-th line. The description of a path is a sequence of cells. Each cell must be written in the format <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, where <span class="tex-span"><i>i</i></span> is the number of the row and <span class="tex-span"><i>j</i></span> is the number of the column. You are allowed to print extra whitespaces in the line. If there are multiple optimal solutions, print any of them.</p><p>Please follow the output format strictly! If your program passes the first pretest, then the output format is correct.</p>





```input1
4 4 4

```




```output1
8
(1,1) (2,1) (2,2)
(1,1) (1,2)
(1,1) (2,1)
(1,1)

```



## Note

<p>Note to the sample. Initially the matrix is empty. Then Inna follows her first path, the path penalty equals the number of cells in it — 3. Note that now no path can go through cell (2, 2), as it now contains a candy. The next two candies go to cells (1, 2) and (2, 1). Inna simply leaves the last candy at cell (1, 1), the path contains only this cell. The total penalty is: 3 + 2 + 2 + 1 = 8.</p><p>Note that Inna couldn't use cell (1, 1) to place, for instance, the third candy as in this case she couldn't have made the path for the fourth candy.</p>
