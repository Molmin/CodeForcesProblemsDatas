## Description

<div><p>Vasiliy finally got to work, where there is a huge amount of tasks waiting for him. Vasiliy is given a matrix consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns and <span class="tex-span"><i>q</i></span> tasks. Each task is to swap two submatrices of the given matrix.</p><p>For each task Vasiliy knows six integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the index of the row where the top-left corner of the first rectangle is located, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the index of its column, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the index of the row of the top-left corner of the second rectangle, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the index of its column, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the height of the rectangle and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is its width.</p><p>It's guaranteed that two rectangles in one query do not overlap and do not touch, that is, no cell belongs to both rectangles, and no two cells belonging to different rectangles <span class="tex-font-style-bf">share a side</span>. However, rectangles are allowed to share an angle.</p><p>Vasiliy wants to know how the matrix will look like after all tasks are performed.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10 000</span>)&nbsp;— the number of rows and columns in matrix, and the number of tasks Vasiliy has to perform.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) each&nbsp;— initial values of the cells of the matrix.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines contains six integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers each&nbsp;— the resulting matrix.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10 000</span>)&nbsp;— the number of rows and columns in matrix, and the number of tasks Vasiliy has to perform.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) each&nbsp;— initial values of the cells of the matrix.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines contains six integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers each&nbsp;— the resulting matrix.</p>





```input1
4 4 2
1 1 2 2
1 1 2 2
3 3 4 4
3 3 4 4
1 1 3 3 2 2
3 1 1 3 2 2

```




```input2
4 2 1
1 1
1 1
2 2
2 2
1 1 4 1 1 2

```




```output1
4 4 3 3
4 4 3 3
2 2 1 1
2 2 1 1

```




```output2
2 2
1 1
2 2
1 1

```


