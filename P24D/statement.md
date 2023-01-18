## Description

<div><p>You received as a gift a very clever robot walking on a rectangular board. Unfortunately, you understood that it is broken and behaves rather strangely (randomly). The board consists of <span class="tex-span"><i>N</i></span> rows and <span class="tex-span"><i>M</i></span> columns of cells. The robot is initially at some cell on the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column. Then at every step the robot could go to some another cell. The aim is to go to the bottommost (<span class="tex-span"><i>N</i></span>-th) row. The robot can stay at it's current cell, move to the left, move to the right, or move to the cell below the current. If the robot is in the leftmost column it cannot move to the left, and if it is in the rightmost column it cannot move to the right. At every step all possible moves are equally probable. Return the expected number of step to reach the bottommost row.</p></div><div class="input-specification"><p>On the first line you will be given two space separated integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 1000</span>). On the second line you will be given another two space separated integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>N</i>, 1 ≤ <i>j</i> ≤ <i>M</i></span>) — the number of the initial row and the number of the initial column. Note that, <span class="tex-span">(1, 1)</span> is the upper left corner of the board and <span class="tex-span">(<i>N</i>, <i>M</i>)</span> is the bottom right corner.</p></div><div class="output-specification"><p>Output the expected number of steps on a line of itself with at least <span class="tex-span">4</span> digits after the decimal point.</p></div>

## Input

<p>On the first line you will be given two space separated integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 1000</span>). On the second line you will be given another two space separated integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>N</i>, 1 ≤ <i>j</i> ≤ <i>M</i></span>) — the number of the initial row and the number of the initial column. Note that, <span class="tex-span">(1, 1)</span> is the upper left corner of the board and <span class="tex-span">(<i>N</i>, <i>M</i>)</span> is the bottom right corner.</p>

## Output

<p>Output the expected number of steps on a line of itself with at least <span class="tex-span">4</span> digits after the decimal point.</p>





```input1
10 10
10 4

```




```input2
10 14
5 14

```




```output1
0.0000000000

```




```output2
18.0038068653

```


