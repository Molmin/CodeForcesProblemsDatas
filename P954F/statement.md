## Description

<div><p>You are running through a rectangular field. This field can be represented as a matrix with <span class="tex-span">3</span> rows and <span class="tex-span"><i>m</i></span> columns. <span class="tex-span">(<i>i</i>, <i>j</i>)</span> denotes a cell belonging to <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column.</p><p>You start in <span class="tex-span">(2, 1)</span> and have to end your path in <span class="tex-span">(2, <i>m</i>)</span>. From the cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> you may advance to:</p><ul> <li> <span class="tex-span">(<i>i</i> - 1, <i>j</i> + 1)</span> — only if <span class="tex-span"><i>i</i> &gt; 1</span>, </li><li> <span class="tex-span">(<i>i</i>, <i>j</i> + 1)</span>, or </li><li> <span class="tex-span">(<i>i</i> + 1, <i>j</i> + 1)</span> — only if <span class="tex-span"><i>i</i> &lt; 3</span>. </li></ul><p>However, there are <span class="tex-span"><i>n</i></span> obstacles blocking your path. <span class="tex-span"><i>k</i></span>-th obstacle is denoted by three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span>, and it forbids entering any cell <span class="tex-span">(<i>a</i><sub class="lower-index"><i>k</i></sub>, <i>j</i>)</span> such that <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>j</i> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>You have to calculate the number of different paths from <span class="tex-span">(2, 1)</span> to <span class="tex-span">(2, <i>m</i>)</span>, and print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">3 ≤ <i>m</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of obstacles and the number of columns in the matrix, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each containing three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 3</span>, <span class="tex-span">2 ≤ <i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub> ≤ <i>m</i> - 1</span>) denoting an obstacle blocking every cell <span class="tex-span">(<i>a</i><sub class="lower-index"><i>k</i></sub>, <i>j</i>)</span> such that <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>j</i> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub></span>. Some cells may be blocked by multiple obstacles.</p></div><div class="output-specification"><p>Print the number of different paths from <span class="tex-span">(2, 1)</span> to <span class="tex-span">(2, <i>m</i>)</span>, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. If it is impossible to get from <span class="tex-span">(2, 1)</span> to <span class="tex-span">(2, <i>m</i>)</span>, then the number of paths is <span class="tex-span">0</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">3 ≤ <i>m</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of obstacles and the number of columns in the matrix, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each containing three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 3</span>, <span class="tex-span">2 ≤ <i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub> ≤ <i>m</i> - 1</span>) denoting an obstacle blocking every cell <span class="tex-span">(<i>a</i><sub class="lower-index"><i>k</i></sub>, <i>j</i>)</span> such that <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>j</i> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub></span>. Some cells may be blocked by multiple obstacles.</p>

## Output

<p>Print the number of different paths from <span class="tex-span">(2, 1)</span> to <span class="tex-span">(2, <i>m</i>)</span>, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. If it is impossible to get from <span class="tex-span">(2, 1)</span> to <span class="tex-span">(2, <i>m</i>)</span>, then the number of paths is <span class="tex-span">0</span>.</p>





```input1
2 5
1 3 4
2 2 3

```




```output1
2

```


