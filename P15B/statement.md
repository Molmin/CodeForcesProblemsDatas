## Description

<div><p>Petya is the most responsible worker in the Research Institute. So he was asked to make a very important experiment: to melt the chocolate bar with a new laser device. The device consists of a rectangular field of <span class="tex-span"><i>n</i> × <i>m</i></span> cells and a robotic arm. Each cell of the field is a <span class="tex-span">1 × 1</span> square. The robotic arm has two lasers pointed at the field perpendicularly to its surface. At any one time lasers are pointed at the centres of some two cells. Since the lasers are on the robotic hand, their movements are synchronized — if you move one of the lasers by a vector, another one moves by the same vector.</p><p>The following facts about the experiment are known: </p><ul> <li> initially the whole field is covered with a chocolate bar of the size <span class="tex-span"><i>n</i> × <i>m</i></span>, both lasers are located above the field and are active; </li><li> the chocolate melts within one cell of the field at which the laser is pointed; </li><li> all moves of the robotic arm should be parallel to the sides of the field, after each move the lasers should be pointed at the centres of some two cells; </li><li> at any one time both lasers should be pointed at the field. Petya doesn't want to become a second Gordon Freeman. </li></ul><p>You are given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and the cells <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, where the lasers are initially pointed at (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is a column number, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is a row number). Rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from top to bottom and columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. You are to find the amount of cells of the field on which the chocolate can't be melted in the given conditions.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10000)</span> — the number of test sets. Each of the following <span class="tex-span"><i>t</i></span> lines describes one test set. Each line contains integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, separated by a space (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>). Cells <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> are distinct.</p></div><div class="output-specification"><p>Each of the <span class="tex-span"><i>t</i></span> lines of the output should contain the answer to the corresponding input test set.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10000)</span> — the number of test sets. Each of the following <span class="tex-span"><i>t</i></span> lines describes one test set. Each line contains integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, separated by a space (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>). Cells <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> are distinct.</p>

## Output

<p>Each of the <span class="tex-span"><i>t</i></span> lines of the output should contain the answer to the corresponding input test set.</p>





```input1
2
4 4 1 1 3 3
4 3 1 1 2 2

```




```output1
8
2

```


