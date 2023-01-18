## Description

<div><p>One day Qwerty the Ranger witnessed two transport ships collide with each other. As a result, all contents of their cargo holds scattered around the space. And now Qwerty wants to pick as many lost items as possible to sell them later.</p><p>The thing is, both ships had lots of new gravitational grippers, transported to sale. A gripper is a device that can be installed on a spaceship and than draw items in space to itself ("grip") and transport them to the ship's cargo hold. </p><p>Overall the crashed ships lost <span class="tex-span"><i>n</i></span> gravitational grippers: the <span class="tex-span"><i>i</i></span>-th gripper is located at a point with coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. Each gripper has two features — <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (the power) and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (the action radius) and can grip any items with mass of no more than <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> at distance no more than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. A gripper itself is an item, too and it has its mass of <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Qwerty's ship is located at point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and has an old magnetic gripper installed, its characteristics are <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>r</i></span>. There are no other grippers in the ship's cargo holds.</p><p>Find the largest number of grippers Qwerty can get hold of. As he picks the items, he can arbitrarily install any gripper in the cargo hold of the ship, including the gripper he has just picked. At any moment of time the ship can have only one active gripper installed. We consider all items and the Qwerty's ship immobile when the ranger picks the items, except for when the gripper moves an item — then the item moves to the cargo holds and the ship still remains immobile. We can assume that the ship's cargo holds have enough room for all grippers. Qwerty can use any gripper he finds or the initial gripper an arbitrary number of times.</p></div><div class="input-specification"><p>The first line contains five integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>p</i>, <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 250000</span>) — the ship's initial position, the initial gripper's features and the number of grippers that got into the space during the collision.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the grippers' descriptions: the <span class="tex-span"><i>i</i></span>-th line contains five integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the <span class="tex-span"><i>i</i></span>-th gripper's coordinates and features.</p><p>It is guaranteed that all grippers are located at different points. No gripper is located at the same point with Qwerty's ship.</p></div><div class="output-specification"><p>Print a single number — the maximum number of grippers Qwerty can draw to his ship. You do not need to count the initial old magnet gripper.</p></div>

## Input

<p>The first line contains five integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>p</i>, <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 250000</span>) — the ship's initial position, the initial gripper's features and the number of grippers that got into the space during the collision.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the grippers' descriptions: the <span class="tex-span"><i>i</i></span>-th line contains five integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the <span class="tex-span"><i>i</i></span>-th gripper's coordinates and features.</p><p>It is guaranteed that all grippers are located at different points. No gripper is located at the same point with Qwerty's ship.</p>

## Output

<p>Print a single number — the maximum number of grippers Qwerty can draw to his ship. You do not need to count the initial old magnet gripper.</p>





```input1
0 0 5 10 5
5 4 7 11 5
-7 1 4 7 8
0 2 13 5 6
2 -3 9 3 4
13 5 1 9 9

```




```output1
3

```



## Note

<p>In the first sample you should get the second gripper, then use the second gripper to get the first one, then use the first gripper to get the fourth one. You cannot get neither the third gripper as it is too heavy, nor the fifth one as it is too far away.</p>
