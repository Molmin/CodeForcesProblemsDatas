## Description

<div><p>Olya loves energy drinks. She loves them so much that her room is full of empty cans from energy drinks.</p><p>Formally, her room can be represented as a field of <span class="tex-span"><i>n</i> × <i>m</i></span> cells, each cell of which is empty or littered with cans.</p><p>Olya drank a lot of energy drink, so now she can run <span class="tex-span"><i>k</i></span> meters per second. Each second she chooses one of the four directions (up, down, left or right) and runs from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span> meters in this direction. Of course, she can only run through empty cells.</p><p>Now Olya needs to get from cell <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> to cell <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>. How many seconds will it take her if she moves optimally?</p><p>It's guaranteed that cells <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> are empty. These cells can coincide.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 1000</span>) — the sizes of the room and Olya's speed.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow containing <span class="tex-span"><i>m</i></span> characters each, the <span class="tex-span"><i>i</i></span>-th of them contains on <span class="tex-span"><i>j</i></span>-th position "<span class="tex-font-style-tt">#</span>", if the cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is littered with cans, and "<span class="tex-font-style-tt">.</span>" otherwise.</p><p>The last line contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — the coordinates of the first and the last cells.</p></div><div class="output-specification"><p>Print a single integer — the minimum time it will take Olya to get from <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> to <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p><p>If it's impossible to get from <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> to <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 1000</span>) — the sizes of the room and Olya's speed.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow containing <span class="tex-span"><i>m</i></span> characters each, the <span class="tex-span"><i>i</i></span>-th of them contains on <span class="tex-span"><i>j</i></span>-th position "<span class="tex-font-style-tt">#</span>", if the cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is littered with cans, and "<span class="tex-font-style-tt">.</span>" otherwise.</p><p>The last line contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — the coordinates of the first and the last cells.</p>

## Output

<p>Print a single integer — the minimum time it will take Olya to get from <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> to <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p><p>If it's impossible to get from <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> to <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
3 4 4
....
###.
....
1 1 3 1

```




```input2
3 4 1
....
###.
....
1 1 3 1

```




```input3
2 2 1
.#
#.
1 1 2 2

```




```output1
3
```




```output2
8
```




```output3
-1
```



## Note

<p>In the first sample Olya should run <span class="tex-span">3</span> meters to the right in the first second, <span class="tex-span">2</span> meters down in the second second and <span class="tex-span">3</span> meters to the left in the third second.</p><p>In second sample Olya should run to the right for <span class="tex-span">3</span> seconds, then down for <span class="tex-span">2</span> seconds and then to the left for <span class="tex-span">3</span> seconds.</p><p><span class="tex-font-style-it">Olya does not recommend drinking energy drinks and generally believes that this is bad</span>.</p>
