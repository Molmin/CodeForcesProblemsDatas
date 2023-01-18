## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Vladik has favorite game, in which he plays all his free time.</p><p>Game field could be represented as <span class="tex-span"><i>n</i> × <i>m</i></span> matrix which consists of cells of three types: </p><ul> <li> «<span class="tex-font-style-tt">.</span>» — normal cell, player can visit it. </li><li> «<span class="tex-font-style-tt">F</span>» — finish cell, player has to finish his way there to win. There is exactly one cell of this type. </li><li> «<span class="tex-font-style-tt">*</span>» — dangerous cell, if player comes to this cell, he loses. </li></ul><p>Initially player is located in the left top cell with coordinates <span class="tex-span">(1, 1)</span>. </p><p>Player has access to <span class="tex-span">4</span> buttons "<span class="tex-font-style-tt">U</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", each of them move player up, down, left and right directions respectively.</p><p>But it’s not that easy! Sometimes friends play game and change functions of buttons. Function of buttons "<span class="tex-font-style-tt">L</span>" and "<span class="tex-font-style-tt">R</span>" could have been swapped, also functions of buttons "<span class="tex-font-style-tt">U</span>" and "<span class="tex-font-style-tt">D</span>" could have been swapped. Note that functions of buttons can be changed only at the beginning of the game.</p><p>Help Vladik win the game!</p></div><div class="input-specification"><p>First line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — number of rows and columns respectively.</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters describing corresponding row of field. Set of characters in field is described above.</p><p>Guaranteed that cell with coordinates <span class="tex-span">(1, 1)</span> is normal and there is at least one way from initial cell to finish cell without dangerous cells. </p></div><div><h2>Interaction</h2><p>You can press buttons no more than <span class="tex-span">2·<i>n</i>·<i>m</i></span> times.</p><p>To press a button you should print "<span class="tex-font-style-tt">U</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" in new line. It’s necessary to print newline character and <span class="tex-font-style-tt">flush</span> output. After flushing buffer you should read answer from input data. Answer is the pair of space-separated integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> — new position of player. In case, if there is no cell in direction of moving, position will not change. If after any move player lost, in other words player move to dangerous cell, then <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> will be equal to <span class="tex-span"> - 1</span>.</p><p>If after any move player is in finish or dangerous cell, then you should terminate your program.</p><p>To finish output buffer (i. e. for operation <span class="tex-font-style-tt">flush</span>) right after printing direction and newline you should do next:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++ </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal </li><li> read documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span> </p><p>To perform a hack you should use this format:</p><pre class="verbatim"><br>n m swapLR swapUD  <br>a_1  <br>a_2  <br>...  <br>a_n<br></pre> <p>Where <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>&nbsp;— number of rows and columns in game field. <span class="tex-span"><i>swapLR</i></span> is equal to <span class="tex-span">1</span> in case, when directions "<span class="tex-font-style-tt">L</span>’’ and "<span class="tex-font-style-tt">R</span>’’ is swapped, and equal to <span class="tex-span">0</span> otherwise. <span class="tex-span"><i>swapUD</i></span> is equal to <span class="tex-span">1</span>, when directions "<span class="tex-font-style-tt">U</span>’’ and "<span class="tex-font-style-tt">D</span>’’ is swapped, and equal to <span class="tex-span">0</span> otherwise. <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — description of corresponding rows of game field.</p></div>

## Input

<p>First line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — number of rows and columns respectively.</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters describing corresponding row of field. Set of characters in field is described above.</p><p>Guaranteed that cell with coordinates <span class="tex-span">(1, 1)</span> is normal and there is at least one way from initial cell to finish cell without dangerous cells. </p>





```input1
4 3
...
**.
F*.
...
1 1
1 2
1 3
1 3
2 3
3 3
4 3
4 2
4 1
3 1

```




```output1
R
L
L
D
U
U
U
R
R
D

```



## Note

<p>In first test case all four directions swapped with their opposite directions. Protocol of interaction In more convenient form:</p><p><img class="tex-graphics" src="file://wYCquxIg.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>This test could be presenter for hack in following way: </p><pre class="verbatim"><br>4 3 1 1<br>...<br>**.<br>F*.<br>...<br></pre>
