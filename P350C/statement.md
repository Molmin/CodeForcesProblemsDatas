## Description

<div><p>You've got a robot, its task is destroying bombs on a square plane. Specifically, the square plane contains <span class="tex-span"><i>n</i></span> bombs, the <span class="tex-span"><i>i</i></span>-th bomb is at point with coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. We know that no two bombs are at the same point and that no bomb is at point with coordinates <span class="tex-span">(0, 0)</span>. Initially, the robot is at point with coordinates <span class="tex-span">(0, 0)</span>. Also, let's mark the robot's current position as <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. In order to destroy all the bombs, the robot can perform three types of operations:</p><ol> <li> Operation has format "<span class="tex-font-style-tt">1 k dir</span>". To perform the operation robot have to move in direction <span class="tex-span"><i>dir</i></span> <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≥ 1</span>) times. There are only <span class="tex-span">4</span> directions the robot can move in: "R", "L", "U", "D". During one move the robot can move from the current point to one of following points: <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> - 1, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> - 1)</span> (corresponding to directions). It is forbidden to move from point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, if at least one point on the path (besides the destination point) contains a bomb. </li><li> Operation has format "<span class="tex-font-style-tt">2</span>". To perform the operation robot have to pick a bomb at point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and put it in a special container. Thus, the robot can carry the bomb from any point to any other point. The operation cannot be performed if point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> has no bomb. It is forbidden to pick a bomb if the robot already has a bomb in its container. </li><li> Operation has format "<span class="tex-font-style-tt">3</span>". To perform the operation robot have to take a bomb out of the container and destroy it. You are allowed to perform this operation only if the robot is at point <span class="tex-span">(0, 0)</span>. It is forbidden to perform the operation if the container has no bomb. </li></ol><p>Help the robot and find the shortest possible sequence of operations he can perform to destroy all bombs on the coordinate plane.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of bombs on the coordinate plane. Next <span class="tex-span"><i>n</i></span> lines contain two integers each. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th bomb. It is guaranteed that no two bombs are located at the same point and no bomb is at point <span class="tex-span">(0, 0)</span>. </p></div><div class="output-specification"><p>In a single line print a single integer <span class="tex-span"><i>k</i></span> — the minimum number of operations needed to destroy all bombs. On the next lines print the descriptions of these <span class="tex-span"><i>k</i></span> operations. If there are multiple sequences, you can print any of them. It is guaranteed that there is the solution where <span class="tex-span"><i>k</i> ≤ 10<sup class="upper-index">6</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of bombs on the coordinate plane. Next <span class="tex-span"><i>n</i></span> lines contain two integers each. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th bomb. It is guaranteed that no two bombs are located at the same point and no bomb is at point <span class="tex-span">(0, 0)</span>. </p>

## Output

<p>In a single line print a single integer <span class="tex-span"><i>k</i></span> — the minimum number of operations needed to destroy all bombs. On the next lines print the descriptions of these <span class="tex-span"><i>k</i></span> operations. If there are multiple sequences, you can print any of them. It is guaranteed that there is the solution where <span class="tex-span"><i>k</i> ≤ 10<sup class="upper-index">6</sup></span>.</p>





```input1
2
1 1
-1 -1

```




```input2
3
5 0
0 5
1 0

```




```output1
12
1 1 R
1 1 U
2
1 1 L
1 1 D
3
1 1 L
1 1 D
2
1 1 R
1 1 U
3

```




```output2
12
1 1 R
2
1 1 L
3
1 5 R
2
1 5 L
3
1 5 U
2
1 5 D
3

```


