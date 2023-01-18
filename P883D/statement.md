## Description

<div><p>Game field is represented by a line of <span class="tex-span"><i>n</i></span> square cells. In some cells there are packmen, in some cells there are asterisks and the rest of the cells are empty. Packmen eat asterisks.</p><p>Before the game starts you can choose a movement direction, left or right, for each packman. Once the game begins all the packmen simultaneously start moving according their directions. A packman can't change the given direction.</p><p>Once a packman enters a cell containing an asterisk, packman immediately eats the asterisk. Once the packman leaves the cell it becomes empty. Each packman moves at speed 1 cell per second. If a packman enters a border cell, the packman stops. Packmen do not interfere with the movement of other packmen; in one cell there can be any number of packmen moving in any directions.</p><p>Your task is to assign a direction to each packman so that they eat the maximal number of asterisks. If there are multiple ways to assign directions to eat the maximal number of asterisks, you should choose the way which minimizes the time to do that.</p></div><div class="input-specification"><p>The first line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000 000</span>) — the number of cells in the game field.</p><p>The second line contains <span class="tex-span"><i>n</i></span> characters. If the <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">.</span>', the <span class="tex-span"><i>i</i></span>-th cell is empty. If the <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">*</span>', the <span class="tex-span"><i>i</i></span>-th cell contains an asterisk. If the <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">P</span>', the <span class="tex-span"><i>i</i></span>-th cell contains a packman.</p><p>The field contains at least one asterisk and at least one packman.</p></div><div class="output-specification"><p>Print two integer numbers — the maximal number of asterisks packmen can eat and the minimal time to do it.</p></div>

## Input

<p>The first line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000 000</span>) — the number of cells in the game field.</p><p>The second line contains <span class="tex-span"><i>n</i></span> characters. If the <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">.</span>', the <span class="tex-span"><i>i</i></span>-th cell is empty. If the <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">*</span>', the <span class="tex-span"><i>i</i></span>-th cell contains an asterisk. If the <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">P</span>', the <span class="tex-span"><i>i</i></span>-th cell contains a packman.</p><p>The field contains at least one asterisk and at least one packman.</p>

## Output

<p>Print two integer numbers — the maximal number of asterisks packmen can eat and the minimal time to do it.</p>





```input1
6
*.P*P*

```




```input2
8
*...P..*

```




```output1
3 4

```




```output2
1 3

```



## Note

<p>In the first example the leftmost packman should move to the right, the rightmost packman should move to the left. All the asterisks will be eaten, the last asterisk will be eaten after 4 seconds.</p>
