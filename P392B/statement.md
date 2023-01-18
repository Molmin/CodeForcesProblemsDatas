## Description

<div><p>The Tower of Hanoi is a well-known mathematical puzzle. It consists of three rods, and a number of disks of different sizes which can slide onto any rod. The puzzle starts with the disks in a neat stack in ascending order of size on one rod, the smallest at the top, thus making a conical shape.</p><p>The objective of the puzzle is to move the entire stack to another rod, obeying the following simple rules: </p><ol> <li> Only one disk can be moved at a time. </li><li> Each move consists of taking the upper disk from one of the stacks and placing it on top of another stack i.e. a disk can only be moved if it is the uppermost disk on a stack. </li><li> No disk may be placed on top of a smaller disk. </li></ol><p>With three disks, the puzzle can be solved in seven moves. The minimum number of moves required to solve a Tower of Hanoi puzzle is <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> - 1</span>, where <span class="tex-span"><i>n</i></span> is the number of disks. (c) Wikipedia.</p><p>SmallY's puzzle is very similar to the famous Tower of Hanoi. In the Tower of Hanoi puzzle you need to solve a puzzle in minimum number of moves, in SmallY's puzzle each move costs some money and you need to solve the same puzzle but for minimal cost. At the beginning of SmallY's puzzle all <span class="tex-span"><i>n</i></span> disks are on the first rod. Moving a disk from rod <span class="tex-span"><i>i</i></span> to rod <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ 3)</span> costs <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> units of money. The goal of the puzzle is to move all the disks to the third rod.</p><p>In the problem you are given matrix <span class="tex-span"><i>t</i></span> and an integer <span class="tex-span"><i>n</i></span>. You need to count the minimal cost of solving SmallY's puzzle, consisting of <span class="tex-span"><i>n</i></span> disks.</p></div><div class="input-specification"><p>Each of the first three lines contains three integers — matrix <span class="tex-span"><i>t</i></span>. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>ij</i></sub> ≤ 10000;&nbsp;<i>i</i> ≠ <i>j</i></span>). The following line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 40)</span> — the number of disks.</p><p>It is guaranteed that for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ 3)</span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>ii</i></sub> = 0</span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum cost of solving SmallY's puzzle.</p></div>

## Input

<p>Each of the first three lines contains three integers — matrix <span class="tex-span"><i>t</i></span>. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>ij</i></sub> ≤ 10000;&nbsp;<i>i</i> ≠ <i>j</i></span>). The following line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 40)</span> — the number of disks.</p><p>It is guaranteed that for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ 3)</span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>ii</i></sub> = 0</span>.</p>

## Output

<p>Print a single integer — the minimum cost of solving SmallY's puzzle.</p>





```input1
0 1 1
1 0 1
1 1 0
3

```




```input2
0 2 2
1 0 100
1 2 0
3

```




```input3
0 2 1
1 0 100
1 2 0
5

```




```output1
7

```




```output2
19

```




```output3
87

```


