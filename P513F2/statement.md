## Description

<div><p>Cthulhu decided to catch Scaygerboss. Scaygerboss found it out and is trying to hide in a pack of his scaygers. Each scayger except Scaygerboss is either a male or a female. Scaygerboss's gender is "other".</p><p>Scaygers are scattered on a two-dimensional map divided into cells. A scayger looks nerdy and loveable if it is staying in the same cell with exactly one scayger of a gender that is different from its own gender. Cthulhu will not be able to catch Scaygerboss if all the scaygers on the map look nerdy and loveable.</p><p>The scaygers can move around at different speeds. For each scayger, we are given the time it takes this scayger to move from a cell to an adjacent cell. Cells are adjacent if they share a common side. At any point of time, each cell that does not contain an obstacle can be occupied by an arbitrary number of scaygers. Scaygers cannot move to cells with obstacles.</p><p>Calculate minimal time in order to make all scaygers look nerdy and loveable if they move optimally toward this goal.</p></div><div class="input-specification"><p>The first line contains 4 integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>males</i></span>, <span class="tex-span"><i>females</i></span> (<span class="tex-span">0 ≤ <i>males</i>, <i>females</i> ≤ <i>n</i>·<i>m</i></span>). <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> are dimensions of the map; <span class="tex-span"><i>males</i></span> and <span class="tex-span"><i>females</i></span> are numbers of male scaygers and female scaygers.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the map. Each of these lines contains <span class="tex-span"><i>m</i></span> characters. Character '.' stands for a free cell; character '#' stands for a cell with an obstacle.</p><p>The next line contains 3 integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span>, and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>): the current coordinates of Scaygerboss and the time it takes Scaygerboss to move to an adjacent cell. The next <span class="tex-span"><i>males</i></span> lines contain coordinates and times of male scaygers in the same format as for Scaygerboss. The next <span class="tex-span"><i>females</i></span> lines contain coordinates and times of female scaygers in the same format as for Scaygerboss. (The coordinates and times adhere to the same limits as for Scaygerboss.) All scaygers reside in cells without obstacles.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem F1 (<span class="tex-span">14</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 11</span> will hold. </li><li> In subproblem F2 (<span class="tex-span">6</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 22</span> will hold. </li></ul></div><div class="output-specification"><p>Output the minimum possible time it takes to make all scaygers look nerdy and loveable or -1 if it is impossible.</p></div>

## Input

<p>The first line contains 4 integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>males</i></span>, <span class="tex-span"><i>females</i></span> (<span class="tex-span">0 ≤ <i>males</i>, <i>females</i> ≤ <i>n</i>·<i>m</i></span>). <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> are dimensions of the map; <span class="tex-span"><i>males</i></span> and <span class="tex-span"><i>females</i></span> are numbers of male scaygers and female scaygers.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the map. Each of these lines contains <span class="tex-span"><i>m</i></span> characters. Character '.' stands for a free cell; character '#' stands for a cell with an obstacle.</p><p>The next line contains 3 integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span>, and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>): the current coordinates of Scaygerboss and the time it takes Scaygerboss to move to an adjacent cell. The next <span class="tex-span"><i>males</i></span> lines contain coordinates and times of male scaygers in the same format as for Scaygerboss. The next <span class="tex-span"><i>females</i></span> lines contain coordinates and times of female scaygers in the same format as for Scaygerboss. (The coordinates and times adhere to the same limits as for Scaygerboss.) All scaygers reside in cells without obstacles.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem F1 (<span class="tex-span">14</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 11</span> will hold. </li><li> In subproblem F2 (<span class="tex-span">6</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 22</span> will hold. </li></ul>

## Output

<p>Output the minimum possible time it takes to make all scaygers look nerdy and loveable or -1 if it is impossible.</p>





```input1
4 4 2 3
....
.###
####
####
2 1 1
2 1 2
2 1 2
2 1 2
2 1 2
1 1 2

```




```input2
2 4 2 2
....
.###
2 1 1
2 1 2
2 1 2
2 1 2
2 1 2

```




```output1
2

```




```output2
-1

```



## Note

<p>Consider the first sample test. The scaygers are hiding on a 4 by 4 map. Scaygerboss initially resides in the cell <span class="tex-span">(2, 1)</span> and can move between cells in 1 unit of time. There are also 2 male and 3 female scaygers on the map. One of the females initially is in the cell <span class="tex-span">(1, 1)</span>, and all the other scaygers are in the cell <span class="tex-span">(2, 1)</span>. All the scaygers move between cells in 2 units of time. If Scaygerboss and the female scayger from the cell <span class="tex-span">(1, 1)</span> move to the cell <span class="tex-span">(1, 2)</span>, and a male and a female scayger from those residing in the cell <span class="tex-span">(2, 1)</span> move to the cell <span class="tex-span">(1, 1)</span>, then all the scaygers will look nerdy and lovable in 2 units of time.</p>
