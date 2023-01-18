## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> rectangles, labeled 1 through <span class="tex-span"><i>n</i></span>. The corners of rectangles have integer coordinates and their edges are parallel to the <span class="tex-span"><i>Ox</i></span> and <span class="tex-span"><i>Oy</i></span> axes. The rectangles may touch each other, but they do not overlap (that is, there are no points that belong to the interior of more than one rectangle).</p><p>Your task is to determine if there's a non-empty subset of the rectangles that forms a square. That is, determine if there exists a subset of the rectangles and some square for which every point that belongs to the interior or the border of that square belongs to the interior or the border of at least one of the rectangles in the subset, and every point that belongs to the interior or the border of at least one rectangle in the subset belongs to the interior or the border of that square.</p></div><div class="input-specification"><p>First line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of rectangles. Each of the next <span class="tex-span"><i>n</i></span> lines contains a description of a rectangle, with the <span class="tex-span"><i>i</i></span>-th such line describing the rectangle labeled <span class="tex-span"><i>i</i></span>. Each rectangle description consists of four integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — coordinates of the bottom left and the top right corners (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 3000</span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> ≤ 3000</span>).</p><p>No two rectangles overlap (that is, there are no points that belong to the interior of more than one rectangle).</p></div><div class="output-specification"><p>If such a subset exists, print "<span class="tex-font-style-tt">YES</span>" (without quotes) on the first line of the output file, followed by <span class="tex-span"><i>k</i></span>, the number of rectangles in the subset. On the second line print <span class="tex-span"><i>k</i></span> numbers — the labels of rectangles in the subset in any order. If more than one such subset exists, print any one. If no such subset exists, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>First line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of rectangles. Each of the next <span class="tex-span"><i>n</i></span> lines contains a description of a rectangle, with the <span class="tex-span"><i>i</i></span>-th such line describing the rectangle labeled <span class="tex-span"><i>i</i></span>. Each rectangle description consists of four integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — coordinates of the bottom left and the top right corners (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 3000</span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> ≤ 3000</span>).</p><p>No two rectangles overlap (that is, there are no points that belong to the interior of more than one rectangle).</p>

## Output

<p>If such a subset exists, print "<span class="tex-font-style-tt">YES</span>" (without quotes) on the first line of the output file, followed by <span class="tex-span"><i>k</i></span>, the number of rectangles in the subset. On the second line print <span class="tex-span"><i>k</i></span> numbers — the labels of rectangles in the subset in any order. If more than one such subset exists, print any one. If no such subset exists, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
9
0 0 1 9
1 0 9 1
1 8 9 9
8 1 9 8
2 2 3 6
3 2 7 3
2 6 7 7
5 3 7 6
3 3 5 6

```




```input2
4
0 0 1 9
1 0 9 1
1 8 9 9
8 1 9 8

```




```output1
YES 5
5 6 7 8 9

```




```output2
NO

```



## Note

<p>The first test case looks as follows:</p><center> <img class="tex-graphics" src="file://mTG2akqK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that rectangles 6, 8, and 9 form a square as well, and would be an acceptable answer.</p><p>The second test case looks as follows:</p><center> <img class="tex-graphics" src="file://tr8AZcum.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
