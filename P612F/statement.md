## Description

<div><p>You are given a circular array with <span class="tex-span"><i>n</i></span> elements. The elements are numbered from some element with values from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in clockwise order. The <span class="tex-span"><i>i</i></span>-th cell contains the value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The robot Simba is in cell <span class="tex-span"><i>s</i></span>.</p><p>Each moment of time the robot is in some of the <span class="tex-span"><i>n</i></span> cells (at the begin he is in <span class="tex-span"><i>s</i></span>). In one turn the robot can write out the number written in current cell or move to the adjacent cell in clockwise or counterclockwise direction. To write out the number from the cell Simba doesn't spend any time, but to move to adjacent cell Simba spends one unit of time.</p><p>Simba wants to write the number from each cell one time, so the numbers will be written in a non decreasing order. Find the least number of time units to write out all numbers.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i> ≤ 2000</span>) — the number of cells in the circular array and the starting position of Simba.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the number written in the <span class="tex-span"><i>i</i></span>-th cell. The numbers are given for cells in order from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> can be equal.</p></div><div class="output-specification"><p>In the first line print the number <span class="tex-span"><i>t</i></span> — the least number of time units.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines should contain the direction of robot movement and the number of cells to move in that direction. After that movement the robot writes out the number from the cell in which it turns out. The direction and the number of cells should be printed in the form of <span class="tex-font-style-tt">+x</span> in case of clockwise movement and <span class="tex-font-style-tt">-x</span> in case of counterclockwise movement to <span class="tex-span"><i>x</i></span> cells (<span class="tex-span">0 ≤ <i>x</i> ≤ <i>n</i> - 1</span>).</p><p>Note that the sum of absolute values of <span class="tex-span"><i>x</i></span> should be equal to <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i> ≤ 2000</span>) — the number of cells in the circular array and the starting position of Simba.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the number written in the <span class="tex-span"><i>i</i></span>-th cell. The numbers are given for cells in order from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> can be equal.</p>

## Output

<p>In the first line print the number <span class="tex-span"><i>t</i></span> — the least number of time units.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines should contain the direction of robot movement and the number of cells to move in that direction. After that movement the robot writes out the number from the cell in which it turns out. The direction and the number of cells should be printed in the form of <span class="tex-font-style-tt">+x</span> in case of clockwise movement and <span class="tex-font-style-tt">-x</span> in case of counterclockwise movement to <span class="tex-span"><i>x</i></span> cells (<span class="tex-span">0 ≤ <i>x</i> ≤ <i>n</i> - 1</span>).</p><p>Note that the sum of absolute values of <span class="tex-span"><i>x</i></span> should be equal to <span class="tex-span"><i>t</i></span>.</p>





```input1
9 1
0 1 2 2 2 1 0 1 1

```




```input2
8 1
0 1 0 1 0 1 0 1

```




```input3
8 1
1 2 3 4 5 6 7 8

```




```input4
8 1
0 0 0 0 0 0 0 0

```




```output1
12
+0
-3
-1
+2
+1
+2
+1
+1
+1

```




```output2
13
+0
+2
+2
+2
-1
+2
+2
+2

```




```output3
7
+0
+1
+1
+1
+1
+1
+1
+1

```




```output4
7
+0
+1
+1
+1
+1
+1
+1
+1

```


