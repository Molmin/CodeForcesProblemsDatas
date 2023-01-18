## Description

<div><p>In this task you have to write a program dealing with nonograms on fields no larger than <span class="tex-span">5 × 20</span>.</p><p>Simplified nonogram is a task where you have to build such field (each cell is either white or black) that satisfies the given information about rows and columns. For each row and each column the number of contiguous black segments is specified. </p><p>For example if size of the field is <span class="tex-span"><i>n</i> = 3, <i>m</i> = 5</span>, аnd numbers of contiguous black segments in rows are: <span class="tex-span">[2, 3, 2]</span> and in columns are: <span class="tex-span">[1, 0, 1, 2, 1]</span> then the solution may look like:</p><center> <img class="tex-graphics" src="file://7O7sExGG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It is guaranteed that on each test in the testset there exists at least one solution.</p></div><div class="input-specification"><p>In the first line there follow two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5, 1 ≤ <i>m</i> ≤ 20</span>) — number of rows and number of columns respectively.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of contiguous black segments in <span class="tex-span"><i>i</i></span>-th row of the field. </p><p>Similarly, third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of contiguous black segments in the <span class="tex-span"><i>i</i></span>-th column of the field.</p><p>It is guaranteed that there exists at least one solution.</p></div><div class="output-specification"><p>Output any possible solution. Output should consist of <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> characters. Denote white cell as "<span class="tex-font-style-tt">.</span>" and black cell as "<span class="tex-font-style-tt">*</span>".</p></div>

## Input

<p>In the first line there follow two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5, 1 ≤ <i>m</i> ≤ 20</span>) — number of rows and number of columns respectively.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of contiguous black segments in <span class="tex-span"><i>i</i></span>-th row of the field. </p><p>Similarly, third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of contiguous black segments in the <span class="tex-span"><i>i</i></span>-th column of the field.</p><p>It is guaranteed that there exists at least one solution.</p>

## Output

<p>Output any possible solution. Output should consist of <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> characters. Denote white cell as "<span class="tex-font-style-tt">.</span>" and black cell as "<span class="tex-font-style-tt">*</span>".</p>





```input1
3 5
2 3 2
1 0 1 2 1

```




```input2
3 3
2 1 2
2 1 2

```




```input3
3 3
1 0 1
2 2 2

```




```output1
*.**.
*.*.*
*..**
```




```output2
*.*
.*.
*.*

```




```output3
***
...
***

```


