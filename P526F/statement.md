## Description

<div><p><span class="tex-font-style-it">In this problem you will meet the simplified model of game Pudding Monsters</span>.</p><p>An important process in developing any game is creating levels. A game field in Pudding Monsters is an <span class="tex-span"><i>n</i> × <i>n</i></span> rectangular grid, <span class="tex-span"><i>n</i></span> of its cells contain monsters and some other cells contain game objects. The gameplay is about moving the monsters around the field. When two monsters are touching each other, they glue together into a single big one (as they are from pudding, remember?).</p><center> <img class="tex-graphics" src="file://8ExTXPU2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Statistics showed that the most interesting maps appear if initially each row and each column contains exactly one monster and the rest of map specifics is set up by the correct positioning of the other game objects. </p><p>A technique that's widely used to make the development process more efficient is reusing the available resources. For example, if there is a large <span class="tex-span"><i>n</i> × <i>n</i></span> map, you can choose in it a smaller <span class="tex-span"><i>k</i> × <i>k</i></span> square part, containing exactly <span class="tex-span"><i>k</i></span> monsters and suggest it as a simplified version of the original map.</p><p>You wonder how many ways there are to choose in the initial map a <span class="tex-span"><i>k</i> × <i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>) square fragment, containing exactly <span class="tex-span"><i>k</i></span> pudding monsters. Calculate this number.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3 × 10<sup class="upper-index">5</sup></span>) — the size of the initial field.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the cells initially containing monsters. The <span class="tex-span"><i>i</i></span>-th of the next lines contains two numbers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the row number and the column number of the cell that initially contains the <span class="tex-span"><i>i</i></span>-th monster.</p><p>It is guaranteed that all <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> are distinct numbers and all <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are distinct numbers.</p></div><div class="output-specification"><p>Print the number of distinct square fragments of the original field that can form a new map.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3 × 10<sup class="upper-index">5</sup></span>) — the size of the initial field.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the cells initially containing monsters. The <span class="tex-span"><i>i</i></span>-th of the next lines contains two numbers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the row number and the column number of the cell that initially contains the <span class="tex-span"><i>i</i></span>-th monster.</p><p>It is guaranteed that all <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> are distinct numbers and all <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are distinct numbers.</p>

## Output

<p>Print the number of distinct square fragments of the original field that can form a new map.</p>





```input1
5
1 1
4 3
3 2
2 4
5 5

```




```output1
10

```


