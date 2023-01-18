## Description

<div><p><span class="tex-font-style-bf">Pay attention to the output section below, where you will see the information about flushing the output.</span></p><p>Bearland is a grid with <span class="tex-span"><i>h</i></span> rows and <span class="tex-span"><i>w</i></span> columns. Rows are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>h</i></span> from top to bottom. Columns are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>w</i></span> from left to right. Every cell is either allowed (denoted by '<span class="tex-font-style-tt">.</span>' in the input) or permanently blocked (denoted by '<span class="tex-font-style-tt">#</span>').</p><p>Bearland is a cold land, where heavy snow often makes travelling harder. Every day a few allowed cells are <span class="tex-font-style-bf">temporarily</span> blocked by snow. Note, that this block works only on this particular day and next day any of these cells might be allowed again (unless there is another temporarily block).</p><p>It's possible to move directly between two cells only if they share a side and none of them is permanently or temporarily blocked.</p><p>Limak is a little polar bear who lives in Bearland. His house is at the top left cell, while his school is at the bottom right cell. Every day Limak should first go from his house to the school and then return back to his house. Since he gets bored easily, he doesn't want to <span class="tex-font-style-bf">visit the same cell twice</span> on one day, except for the cell with his house, where he starts and ends. If Limak can reach a school and return home avoiding revisiting cells, he calls a day <span class="tex-font-style-it">interesting</span>.</p><p>There are <span class="tex-span"><i>q</i></span> days you must process, one after another. For each of these days you should check if it's interesting and print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" on a separate line. In order to be able to read the description of the next day you should print the answer for the previous one and flush the output.</p><p>It's guaranteed that a day with no cells temporarily blocked by snow would be interesting. It's also guaranteed that cells with Limak's house and school are never blocked (neither permanently or temporarily).</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>h</i>, <i>w</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10 000</span>)&nbsp;— the height and the width of the grid, and the number of days, respectively.</p><p>Next <span class="tex-span"><i>h</i></span> lines describe which cells are allowed and which permanently blocked. The <span class="tex-span"><i>i</i></span>-th line contains a string of length <span class="tex-span"><i>w</i></span>, describing the <span class="tex-span"><i>i</i></span>-th row. Every character is either '<span class="tex-font-style-tt">.</span>' (denoting an allowed cell) or '<span class="tex-font-style-tt">#</span>' (denoting a permanently blocked cell). It's guaranteed that a day with no cells temporarily blocked by snow would be interesting.</p><p>Then, the description of <span class="tex-span"><i>q</i></span> days is given. The description of the <span class="tex-span"><i>i</i></span>-th day starts with a line containing a single integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>)&nbsp;— the number of cells that are temporarily blocked by snow on that day. Each of next <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> lines contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>h</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>w</i></span>), representing a cell at the intersection of the row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> and the column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. The given <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> cells are distinct and none of them is permanently blocked. Also, none of them contains Limak's house or school.</p></div><div class="output-specification"><p>For each of <span class="tex-span"><i>q</i></span> days print "<span class="tex-font-style-tt">YES</span>" if that day is interesting, and otherwise print "<span class="tex-font-style-tt">NO</span>", both without the quotes. After printing an answer, you have to both print the end-of-line character and <span class="tex-font-style-tt">flush</span> the output. Then you can proceed to the next day. You can get <span class="tex-font-style-tt">Idleness Limit Exceeded</span> if you don't print anything or if you forget to flush the output.</p><p>To flush you can use (just after printing a <span class="tex-font-style-tt">YES/NO</span> and end-of-line): </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> See the documentation for other languages. </li></ul></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>h</i>, <i>w</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10 000</span>)&nbsp;— the height and the width of the grid, and the number of days, respectively.</p><p>Next <span class="tex-span"><i>h</i></span> lines describe which cells are allowed and which permanently blocked. The <span class="tex-span"><i>i</i></span>-th line contains a string of length <span class="tex-span"><i>w</i></span>, describing the <span class="tex-span"><i>i</i></span>-th row. Every character is either '<span class="tex-font-style-tt">.</span>' (denoting an allowed cell) or '<span class="tex-font-style-tt">#</span>' (denoting a permanently blocked cell). It's guaranteed that a day with no cells temporarily blocked by snow would be interesting.</p><p>Then, the description of <span class="tex-span"><i>q</i></span> days is given. The description of the <span class="tex-span"><i>i</i></span>-th day starts with a line containing a single integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>)&nbsp;— the number of cells that are temporarily blocked by snow on that day. Each of next <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> lines contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>h</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>w</i></span>), representing a cell at the intersection of the row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> and the column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. The given <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> cells are distinct and none of them is permanently blocked. Also, none of them contains Limak's house or school.</p>

## Output

<p>For each of <span class="tex-span"><i>q</i></span> days print "<span class="tex-font-style-tt">YES</span>" if that day is interesting, and otherwise print "<span class="tex-font-style-tt">NO</span>", both without the quotes. After printing an answer, you have to both print the end-of-line character and <span class="tex-font-style-tt">flush</span> the output. Then you can proceed to the next day. You can get <span class="tex-font-style-tt">Idleness Limit Exceeded</span> if you don't print anything or if you forget to flush the output.</p><p>To flush you can use (just after printing a <span class="tex-font-style-tt">YES/NO</span> and end-of-line): </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> See the documentation for other languages. </li></ul>





```input1
3 5 4
.....
.....
.#...
1
1 4
1
1 5
2
2 4
3 1
2
1 5
3 3

```




```input2
9 31 5
...............................
...............................
.###.###.#.###...###.###.#.###.
...#.#.#.#.#.......#.#.#.#...#.
.###.#.#.#.###...###.#.#.#...#.
.#...#.#.#.#.#...#...#.#.#...#.
.###.###.#.###...###.###.#...#.
...............................
...............................
5
6 5
2 11
1 14
8 15
2 14
5
2 14
1 14
8 16
6 5
2 11
3
2 2
1 4
8 30
10
3 1
3 11
5 16
7 21
4 16
3 5
7 31
3 9
7 25
3 27
10
3 1
3 9
7 25
3 27
7 21
4 17
3 5
7 31
4 16
3 11

```




```output1
NO
YES
YES
NO

```




```output2
NO
YES
YES
YES
NO

```



## Note

<p>In the first sample, there are <span class="tex-span">4</span> days. Drawings below show how Limak could go to school and return to his home in the second and the third day (on the left and on the right respectively). A permanently blocked cell is painted red, while cells temporarily blocked by snow are painted orange. Black and green arrows should Limak's way to the school and back to the house respectively.</p><center> <img class="tex-graphics" src="file://pINbrW0x.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the second sample, below you can see how the grid looks like on each day, where '<span class="tex-font-style-tt">#</span>' denotes a cell that is blocked, either temporarily or permanently.</p><center> <img class="tex-graphics" src="file://p3ZBWju9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
