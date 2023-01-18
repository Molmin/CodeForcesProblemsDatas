## Description

<div><p>Filya just learned new geometry object&nbsp;— rectangle. He is given a field consisting of <span class="tex-span"><i>n</i> × <i>n</i></span> unit cells. Rows are numbered from bottom to top with integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Columns are numbered from left to right with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Cell, located at the intersection of the row <span class="tex-span"><i>r</i></span> and column <span class="tex-span"><i>c</i></span> is denoted as <span class="tex-span">(<i>r</i>, <i>c</i>)</span>. Filya has painted two rectangles, such that their sides are parallel to coordinate axes and each cell lies fully inside or fully outside each of them. Moreover, no cell lies in both rectangles.</p><p>Later, hedgehog Filya became interested in the location of his rectangles but was unable to find the sheet of paper they were painted on. They were taken by Sonya and now she wants to play a little game with Filya. He tells her a query rectangle and she replies with the number of initial rectangles that lie <span class="tex-font-style-bf">fully inside</span> the given query rectangle. The query rectangle should match the same conditions as initial rectangles. Rectangle lies fully inside the query if each o its cells lies inside the query.</p><p>Filya knows Sonya really well, so is sure that if he asks more than <span class="tex-span">200</span> questions she will stop to reply.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2<sup class="upper-index">16</sup></span>)&nbsp;— size of the field.</p><p>For each query an integer between <span class="tex-span">0</span> and <span class="tex-span">2</span> is returned&nbsp;— the number of initial rectangles that lie fully inside the query rectangle.</p></div><div class="output-specification"><p>To make a query you have to print "<span class="tex-font-style-tt">?</span> <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>" (without quotes) (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>), where <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> stands for the position of the bottom left cell of the query and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> stands for the up right cell of the query. You are allowed to ask no more than <span class="tex-span">200</span> queries. After each query you should perform "flush" operation and read the answer.</p><p>In case you suppose you've already determined the location of two rectangles (or run out of queries) you should print "<span class="tex-font-style-tt">!</span> <span class="tex-span"><i>x</i><sub class="lower-index">11</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">11</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">12</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">12</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">21</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">21</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">22</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">22</sub></span>" (without quotes), where first four integers describe the bottom left and up right cells of the first rectangle, and following four describe the corresponding cells of the second rectangle. You can print the rectangles in an arbitrary order. After you have printed the answer, print the end of the line and perform "flush". Your program should terminate immediately after it print the answer.</p></div><div><h2>Interaction</h2><p>To flush you can use (just after printing an integer and end-of-line): </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> See the documentation for other languages. </li></ul><p>You will get the <span class="tex-font-style-tt">Wrong Answer</span> verdict if you ask more than <span class="tex-span">200</span> queries, or if you print an incorrect coordinates.</p><p>You will get the <span class="tex-font-style-tt">Idleness Limit Exceeded</span> verdict if you don't print anything (but you should) or if you forget about flushing the output (more info below).</p><p><span class="tex-font-style-bf">Hacking.</span></p><p>The first line should contain an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2<sup class="upper-index">16</sup></span>).</p><p>The second line should contain four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>)&nbsp;— the description of the first rectangle.</p><p>The third line contains the description of the second rectangle in the similar way.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2<sup class="upper-index">16</sup></span>)&nbsp;— size of the field.</p><p>For each query an integer between <span class="tex-span">0</span> and <span class="tex-span">2</span> is returned&nbsp;— the number of initial rectangles that lie fully inside the query rectangle.</p>

## Output

<p>To make a query you have to print "<span class="tex-font-style-tt">?</span> <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>" (without quotes) (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>), where <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> stands for the position of the bottom left cell of the query and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> stands for the up right cell of the query. You are allowed to ask no more than <span class="tex-span">200</span> queries. After each query you should perform "flush" operation and read the answer.</p><p>In case you suppose you've already determined the location of two rectangles (or run out of queries) you should print "<span class="tex-font-style-tt">!</span> <span class="tex-span"><i>x</i><sub class="lower-index">11</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">11</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">12</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">12</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">21</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">21</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">22</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">22</sub></span>" (without quotes), where first four integers describe the bottom left and up right cells of the first rectangle, and following four describe the corresponding cells of the second rectangle. You can print the rectangles in an arbitrary order. After you have printed the answer, print the end of the line and perform "flush". Your program should terminate immediately after it print the answer.</p>





```input1
5
2
1
0
1
1
1
0
1

```




```output1
? 1 1 5 5
? 1 1 3 3
? 1 1 3 1
? 2 2 2 2
? 3 3 5 5
? 3 3 3 5
? 3 3 3 4
? 3 4 3 5
! 2 2 2 2 3 4 3 5

```


