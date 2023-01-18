## Description

<div><p>After some programming contest Roma decided to try himself in tourism. His home country Uzhlyandia is a Cartesian plane. He wants to walk along each of the Main Straight Lines in Uzhlyandia. It is known that each of these lines is a straight line parallel to one of the axes (i.e. it is described with the equation <span class="tex-span"><i>x</i> = <i>a</i></span> or <span class="tex-span"><i>y</i> = <i>a</i></span>, where <span class="tex-span"><i>a</i></span> is integer called the coordinate of this line).</p><p>Roma lost his own map, so he should find out the coordinates of all lines at first. Uncle Anton agreed to help him, using the following rules: </p><ul> <li> Initially Roma doesn't know the number of vertical and horizontal lines and their coordinates; </li><li> Roma can announce integer coordinates of some point in Uzhlandia, and Anton then will tell him the minimum among the distances from the chosen point to each of the lines. However, since the coordinates of the lines don't exceed <span class="tex-span">10<sup class="upper-index">8</sup></span> by absolute value, Roma can't choose a point with coordinates exceeding <span class="tex-span">10<sup class="upper-index">8</sup></span> by absolute value. </li></ul><p>Uncle Anton is in a hurry to the UOI (Uzhlandian Olympiad in Informatics), so he can only answer no more than <span class="tex-span">3·10<sup class="upper-index">5</sup></span> questions.</p><p>The problem is that Roma doesn't know how to find out the coordinates of the lines. Write a program that plays Roma's role and finds the coordinates.</p></div><div class="input-specification"><p>There is no input initially. Your program should make queries to get information.</p><p>It is guaranteed that the number of horizontal and vertical lines is at least <span class="tex-span">1</span> and less than or equal to <span class="tex-span">10<sup class="upper-index">4</sup></span> for each type.</p></div><div><h2>Interaction</h2><p>To make a query, print a line "<span class="tex-font-style-tt">0 x y</span>" (-<span class="tex-span">10<sup class="upper-index">8</sup> ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">8</sup></span>), where <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are the coordinates of the point. After each query you need to print end-of-line, make "<span class="tex-font-style-tt">flush</span>" operation, and then read the answer to the query&nbsp;— the minimum among the distances prom this point to the Main Straight Lines of Uzhlyandia.</p><p>You can do no more than <span class="tex-span">3·10<sup class="upper-index">5</sup></span> queries.</p><p>When you are ready to print the answer, print three lines:</p><ol> <li> In the first line print "<span class="tex-font-style-tt">1 n m</span>", where <span class="tex-span"><i>n</i></span> is the number of vertical lines (parallel to <span class="tex-span"><i>OY</i></span>), and <span class="tex-span"><i>m</i></span> is the number of horizontal lines (parallel to <span class="tex-span"><i>OX</i></span>). </li><li> In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;— the coordinates of the vertical lines. </li><li> In the third line in the same format print <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span>&nbsp;— the coordinates of the horizontal lines. </li></ol><p>You can print coordinates in arbitrary order.</p><p>To make "<span class="tex-font-style-tt">flush</span>", you can use (just after printing a query/answer and end-of-line):</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> see the documentation for other languages. </li></ul><p>You will get <span class="tex-font-style-tt">Wrong Answer</span> if you make more queries than allowed or make an invalid query. </p><p>You can get <span class="tex-font-style-tt">Idleness Limit Exceeded</span> if you don't print anything or if you forget to flush the output.</p><p>If at any moment your program reads <span class="tex-font-style-tt">-1</span> as an answer, it should immediately exit normally (for example, by calling <span class="tex-font-style-tt">exit(0)</span>). You will get <span class="tex-font-style-tt">Wrong Answer</span> in this case, it means that you made more queries than allowed, or made an invalid query. If you ignore this, you can get other verdicts since your program will continue to read from a closed stream.</p><p><span class="tex-font-style-bf">Making test for hacking</span></p><p>The first line should contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>The second line should contain <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (-<span class="tex-span">10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the coordinates of the vertical lines.</p><p>The third line should contain <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (-<span class="tex-span">10<sup class="upper-index">8</sup> ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the coordinates of the horizontal lines.</p><p>You can write coordinates in arbitrary order.</p><p>You can see the example case in the notes.</p></div>

## Input

<p>There is no input initially. Your program should make queries to get information.</p><p>It is guaranteed that the number of horizontal and vertical lines is at least <span class="tex-span">1</span> and less than or equal to <span class="tex-span">10<sup class="upper-index">4</sup></span> for each type.</p>





```input1
1
1
3
2

```




```output1
0 1 2
0 -2 -2
0 5 6
0 -2 2
1 1 2
2
0 -3

```



## Note

<p>The example test is </p><pre class="verbatim"><br>1 2<br>2<br>0 -3<br></pre><p>The minimum distances are:</p><ul> <li> from <span class="tex-span">(1, 2)</span> to <span class="tex-span"><i>x</i> = 2</span>; </li><li> from <span class="tex-span">( - 2,  - 2)</span> to <span class="tex-span"><i>y</i> =  - 3</span>; </li><li> from <span class="tex-span">(5, 6)</span> to <span class="tex-span"><i>x</i> = 2</span>; </li><li> from <span class="tex-span">( - 2, 2)</span> to <span class="tex-span"><i>y</i> = 0</span>. </li></ul>
