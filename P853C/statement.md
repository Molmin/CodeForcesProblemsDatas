## Description

<div><p>Ilya is sitting in a waiting area of Metropolis airport and is bored of looking at time table that shows again and again that his plane is delayed. So he took out a sheet of paper and decided to solve some problems.</p><p>First Ilya has drawn a grid of size <span class="tex-span"><i>n</i> × <i>n</i></span> and marked <span class="tex-span"><i>n</i></span> squares on it, such that no two marked squares share the same row or the same column. He calls a rectangle on a grid with sides parallel to grid sides <span class="tex-font-style-it">beautiful</span> if exactly two of its corner squares are marked. There are exactly <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2</span> beautiful rectangles.</p><p>Ilya has chosen <span class="tex-span"><i>q</i></span> query rectangles on a grid with sides parallel to grid sides (not necessarily beautiful ones), and for each of those rectangles he wants to find its <span class="tex-font-style-it">beauty degree</span>. Beauty degree of a rectangle is the number of beautiful rectangles that share at least one square with the given one.</p><p>Now Ilya thinks that he might not have enough time to solve the problem till the departure of his flight. You are given the description of marked cells and the query rectangles, help Ilya find the beauty degree of each of the query rectangles.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the size of the grid and the number of query rectangles.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, separated by spaces (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are different), they specify grid squares marked by Ilya: in column <span class="tex-span"><i>i</i></span> he has marked a square at row <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, bottom to top, columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, left to right.</p><p>The following <span class="tex-span"><i>q</i></span> lines describe query rectangles. Each rectangle is described by four integers: <span class="tex-span"><i>l</i>, <i>d</i>, <i>r</i>, <i>u</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>d</i> ≤ <i>u</i> ≤ <i>n</i></span>), here <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> are the leftmost and the rightmost columns of the rectangle, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>u</i></span> the bottommost and the topmost rows of the rectangle.</p></div><div class="output-specification"><p>For each query rectangle output its beauty degree on a separate line.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the size of the grid and the number of query rectangles.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, separated by spaces (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are different), they specify grid squares marked by Ilya: in column <span class="tex-span"><i>i</i></span> he has marked a square at row <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, bottom to top, columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, left to right.</p><p>The following <span class="tex-span"><i>q</i></span> lines describe query rectangles. Each rectangle is described by four integers: <span class="tex-span"><i>l</i>, <i>d</i>, <i>r</i>, <i>u</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>d</i> ≤ <i>u</i> ≤ <i>n</i></span>), here <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> are the leftmost and the rightmost columns of the rectangle, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>u</i></span> the bottommost and the topmost rows of the rectangle.</p>

## Output

<p>For each query rectangle output its beauty degree on a separate line.</p>





```input1
2 3
1 2
1 1 1 1
1 1 1 2
1 1 2 2

```




```input2
4 2
1 3 2 4
4 1 4 4
1 1 2 3

```




```output1
1
1
1

```




```output2
3
5

```



## Note

<p>The first sample test has one beautiful rectangle that occupies the whole grid, therefore the answer to any query is 1.</p><p>In the second sample test the first query rectangle intersects 3 beautiful rectangles, as shown on the picture below:</p><p><img class="tex-graphics" src="file://9DD3gic1.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://yYoZxahR.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://3T4iqKwj.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There are 5 beautiful rectangles that intersect the second query rectangle, as shown on the following picture:</p><p><img class="tex-graphics" src="file://iWmflHIY.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://RMRJKsh8.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://MDjABtqj.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://1EUzSpIk.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://Vl7XqYmr.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
