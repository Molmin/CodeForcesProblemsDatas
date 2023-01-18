## Description

<div><p>Owl Sonya gave a huge lake puzzle of size <span class="tex-span"><i>n</i> × <i>m</i></span> to hedgehog Filya as a birthday present. Friends immediately started to assemble the puzzle, but some parts of it turned out to be empty&nbsp;— there was no picture on them. Parts with picture on it are denoted by <span class="tex-span">1</span>, while empty parts are denoted by <span class="tex-span">0</span>. Rows of the puzzle are numbered from top to bottom with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, while columns are numbered from left to right with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p><p>Animals decided to complete the picture and play with it, as it might be even more fun! Owl and hedgehog ask each other some queries. Each query is provided by four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> which define the rectangle, where <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> stands for the coordinates of the up left cell of the rectangle, while <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> stands for the coordinates of the bottom right cell. The answer to the query is the size of the maximum <span class="tex-font-style-bf">square</span> consisting of picture parts only (only parts denoted by <span class="tex-span">1</span>) and located fully inside the query rectangle.</p><p>Help Sonya and Filya answer <span class="tex-span"><i>t</i></span> queries.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— sizes of the puzzle.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>. Each of them is equal to <span class="tex-span">1</span> if the corresponding cell contains a picture and <span class="tex-span">0</span> if it's empty.</p><p>Next line contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1 000 000</span>)&nbsp;— the number of queries.</p><p>Then follow <span class="tex-span"><i>t</i></span> lines with queries' descriptions. Each of them contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>)&nbsp;— coordinates of the up left and bottom right cells of the query rectangle.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain the maximum size of the square consisting of <span class="tex-span">1</span>-s and lying fully inside the query rectangle.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— sizes of the puzzle.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>. Each of them is equal to <span class="tex-span">1</span> if the corresponding cell contains a picture and <span class="tex-span">0</span> if it's empty.</p><p>Next line contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1 000 000</span>)&nbsp;— the number of queries.</p><p>Then follow <span class="tex-span"><i>t</i></span> lines with queries' descriptions. Each of them contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>)&nbsp;— coordinates of the up left and bottom right cells of the query rectangle.</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain the maximum size of the square consisting of <span class="tex-span">1</span>-s and lying fully inside the query rectangle.</p>





```input1
3 4
1 1 0 1
0 1 1 0
0 1 1 0
5
1 1 2 3
2 1 3 2
3 2 3 4
1 1 3 4
1 2 3 4

```




```output1
1
1
1
2
2

```


