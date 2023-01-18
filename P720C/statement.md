## Description

<div><p>Today Peter has got an additional homework for tomorrow. The teacher has given three integers to him: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span>, and asked him to mark one or more squares on a square grid of size <span class="tex-span"><i>n</i> × <i>m</i></span>. </p><p>The marked squares must form a connected figure, and there must be exactly <span class="tex-span"><i>k</i></span> triples of marked squares that form an L-shaped tromino&nbsp;— all three squares are inside a <span class="tex-span">2 × 2</span> square.</p><p>The set of squares forms a connected figure if it is possible to get from any square to any other one if you are allowed to move from a square to any adjacent by a common side square.</p><p>Peter cannot fulfill the task, so he asks you for help. Help him to create such figure.</p></div><div class="input-specification"><p>Input data contains one or more test cases. The first line contains the number of test cases <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>).</p><p>Each of the following <span class="tex-span"><i>t</i></span> test cases is described by a line that contains three integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i></span>, <span class="tex-span"><i>n</i> × <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The sum of values of <span class="tex-span"><i>n</i> × <i>m</i></span> for all tests in one input data doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>For each test case print the answer.</p><p>If it is possible to create such figure, print <span class="tex-span"><i>n</i></span> lines, <span class="tex-span"><i>m</i></span> characters each, use asterisk '*' to denote the marked square, and dot '.' to denote the unmarked one.</p><p>If there is no solution, print <span class="tex-font-style-tt">-1</span>.</p><p>Print empty line between test cases.</p></div>

## Input

<p>Input data contains one or more test cases. The first line contains the number of test cases <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>).</p><p>Each of the following <span class="tex-span"><i>t</i></span> test cases is described by a line that contains three integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i></span>, <span class="tex-span"><i>n</i> × <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The sum of values of <span class="tex-span"><i>n</i> × <i>m</i></span> for all tests in one input data doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>For each test case print the answer.</p><p>If it is possible to create such figure, print <span class="tex-span"><i>n</i></span> lines, <span class="tex-span"><i>m</i></span> characters each, use asterisk '*' to denote the marked square, and dot '.' to denote the unmarked one.</p><p>If there is no solution, print <span class="tex-font-style-tt">-1</span>.</p><p>Print empty line between test cases.</p>





```input1
3
3 3 4
3 3 5
3 3 3

```




```output1
.*.
***
.*.

**.
**.
*..

.*.
***
*..

```


