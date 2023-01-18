## Description

<div><p>Once Vasya and Petya assembled a figure of <span class="tex-span"><i>m</i></span> cubes, each of them is associated with a number between <span class="tex-span">0</span> and <span class="tex-span"><i>m</i> - 1</span> (inclusive, each number appeared exactly once). Let's consider a coordinate system such that the <span class="tex-span"><i>OX</i></span> is the ground, and the <span class="tex-span"><i>OY</i></span> is directed upwards. Each cube is associated with the coordinates of its lower left corner, these coordinates are integers for each cube.</p><p>The figure turned out to be <span class="tex-font-style-underline">stable</span>. This means that for any cube that is not on the ground, there is at least one cube under it such that those two cubes touch <span class="tex-font-style-bf">by a side or a corner</span>. More formally, this means that for the cube with coordinates <span class="tex-span">(<i>x</i>, <i>y</i>)</span> either <span class="tex-span"><i>y</i> = 0</span>, or there is a cube with coordinates <span class="tex-span">(<i>x</i> - 1, <i>y</i> - 1)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> - 1)</span> or <span class="tex-span">(<i>x</i> + 1, <i>y</i> - 1)</span>.</p><p>Now the boys want to disassemble the figure and put all the cubes in a row. In one step the cube is removed from the figure and being put to the right of the blocks that have already been laid. The guys remove the cubes in such order that the figure remains stable. To make the process more interesting, the guys decided to play the following game. The guys take out the cubes from the figure in turns. It is easy to see that after the figure is disassembled, the integers written on the cubes form a number, written in the <span class="tex-span"><i>m</i></span>-ary positional numerical system (possibly, with a leading zero). Vasya wants the resulting number to be maximum possible, and Petya, on the contrary, tries to make it as small as possible. Vasya starts the game.</p><p>Your task is to determine what number is formed after the figure is disassembled, if the boys play optimally. Determine the remainder of the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 9</span>.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the coordinates of the cubes <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in ascending order of numbers written on them. It is guaranteed that the original figure is stable.</p><p>No two cubes occupy the same place.</p></div><div class="output-specification"><p>In the only line print the answer to the problem.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the coordinates of the cubes <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in ascending order of numbers written on them. It is guaranteed that the original figure is stable.</p><p>No two cubes occupy the same place.</p>

## Output

<p>In the only line print the answer to the problem.</p>





```input1
3
2 1
1 0
0 1

```




```input2
5
0 0
0 1
0 2
0 3
0 4

```




```output1
19

```




```output2
2930

```


