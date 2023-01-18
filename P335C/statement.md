## Description

<div><p>In a far away land, there are two cities near a river. One day, the cities decide that they have too little space and would like to reclaim some of the river area into land.</p><p>The river area can be represented by a grid with <span class="tex-span"><i>r</i></span> rows and exactly two columns — each cell represents a rectangular area. The rows are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>r</i></span> from top to bottom, while the columns are numbered <span class="tex-span">1</span> and <span class="tex-span">2</span>.</p><p>Initially, all of the cells are occupied by the river. The plan is to turn some of those cells into land one by one, with the cities alternately choosing a cell to reclaim, and continuing until no more cells can be reclaimed.</p><p>However, the river is also used as a major trade route. The cities need to make sure that ships will still be able to sail from one end of the river to the other. More formally, if a cell <span class="tex-span">(<i>r</i>, <i>c</i>)</span> has been reclaimed, it is not allowed to reclaim any of the cells <span class="tex-span">(<i>r</i> - 1, 3 - <i>c</i>)</span>, <span class="tex-span">(<i>r</i>, 3 - <i>c</i>)</span>, or <span class="tex-span">(<i>r</i> + 1, 3 - <i>c</i>)</span>.</p><p>The cities are not on friendly terms, and each city wants to be the last city to reclaim a cell (they don't care about how many cells they reclaim, just who reclaims a cell last). The cities have already reclaimed <span class="tex-span"><i>n</i></span> cells. Your job is to determine which city will be the last to reclaim a cell, assuming both choose cells optimally from current moment.</p></div><div class="input-specification"><p>The first line consists of two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 100, 0 ≤ <i>n</i> ≤ <i>r</i></span>). Then <span class="tex-span"><i>n</i></span> lines follow, describing the cells that were already reclaimed. Each line consists of two integers: <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), which represent the cell located at row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. All of the lines describing the cells will be distinct, and the reclaimed cells will not violate the constraints above.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">WIN</span>" if the city whose turn it is to choose a cell can guarantee that they will be the last to choose a cell. Otherwise print "<span class="tex-font-style-tt">LOSE</span>".</p></div>

## Input

<p>The first line consists of two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 100, 0 ≤ <i>n</i> ≤ <i>r</i></span>). Then <span class="tex-span"><i>n</i></span> lines follow, describing the cells that were already reclaimed. Each line consists of two integers: <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), which represent the cell located at row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. All of the lines describing the cells will be distinct, and the reclaimed cells will not violate the constraints above.</p>

## Output

<p>Output "<span class="tex-font-style-tt">WIN</span>" if the city whose turn it is to choose a cell can guarantee that they will be the last to choose a cell. Otherwise print "<span class="tex-font-style-tt">LOSE</span>".</p>





```input1
3 1
1 1

```




```input2
12 2
4 1
8 1

```




```input3
1 1
1 2

```




```output1
WIN

```




```output2
WIN

```




```output3
LOSE

```



## Note

<p>In the first example, there are 3 possible cells for the first city to reclaim: <span class="tex-span">(2, 1)</span>, <span class="tex-span">(3, 1)</span>, or <span class="tex-span">(3, 2)</span>. The first two possibilities both lose, as they leave exactly one cell for the other city.</p><center> <img class="tex-graphics" src="file://TGOuszBG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>However, reclaiming the cell at <span class="tex-span">(3, 2)</span> leaves no more cells that can be reclaimed, and therefore the first city wins.</p><center> <img class="tex-graphics" src="file://7Ik04IA4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third example, there are no cells that can be reclaimed.</p>
