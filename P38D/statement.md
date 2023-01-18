## Description

<div><p>Once Vasya played bricks. All the bricks in the set had regular cubical shape. Vasya vas a talented architect, however the tower he built kept falling apart.</p><p>Let us consider the building process. Vasya takes a brick and puts it on top of the already built tower so that the sides of the brick are parallel to the sides of the bricks he has already used. Let's introduce a Cartesian coordinate system on the horizontal plane, where Vasya puts the first brick. Then the projection of brick number <span class="tex-span"><i>i</i></span> on the plane is a square with sides parallel to the axes of coordinates with opposite corners in points <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 2</sub>)</span>. The bricks are cast from homogeneous plastic and the weight of a brick <span class="tex-span"><i>a</i> × <i>a</i> × <i>a</i></span> is <span class="tex-span"><i>a</i><sup class="upper-index">3</sup></span> grams.</p><p>It is guaranteed that Vasya puts any brick except the first one on the previous one, that is the area of intersection of the upper side of the previous brick and the lower side of the next brick is always positive.</p><p>We (Vasya included) live in a normal world where the laws of physical statics work. And that is why, perhaps, if we put yet another brick, the tower will collapse under its own weight. Vasya puts the cubes consecutively one on top of the other until at least one cube loses the balance and falls down. If it happens, Vasya gets upset and stops the construction. Print the number of bricks in the maximal stable tower, that is the maximal number <span class="tex-span"><i>m</i></span> satisfying the condition that all the towers consisting of bricks 1, 2, ..., <span class="tex-span"><i>k</i></span> for every integer <span class="tex-span"><i>k</i></span> from 1 to <span class="tex-span"><i>m</i></span> remain stable.</p></div><div class="input-specification"><p>The first input file contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) which is the number of bricks. Each of the next <span class="tex-span"><i>n</i></span> lines contains four numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 2</sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub> ≠ <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, |<i>x</i><sub class="lower-index"><i>i</i>, 1</sub> - <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>| = |<i>y</i><sub class="lower-index"><i>i</i>, 1</sub> - <i>y</i><sub class="lower-index"><i>i</i>, 2</sub>|</span>) which are the coordinates of the opposite angles of the base of the brick number <span class="tex-span"><i>i</i></span>. The coordinates are integers and their absolute value does not exceed <span class="tex-span">50</span>. </p><p>The cubes are given in the order Vasya puts them. It is guaranteed that the area of intersection of the upper side of the brick number <span class="tex-span"><i>i</i> - 1</span> and the lower side of the brick number <span class="tex-span"><i>i</i></span> is strictly strictly greater than zero for all <span class="tex-span"><i>i</i> ≥ 2</span>.</p></div><div class="output-specification"><p>Print the number of bricks in the maximal stable tower.</p></div>

## Input

<p>The first input file contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) which is the number of bricks. Each of the next <span class="tex-span"><i>n</i></span> lines contains four numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 2</sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub> ≠ <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, |<i>x</i><sub class="lower-index"><i>i</i>, 1</sub> - <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>| = |<i>y</i><sub class="lower-index"><i>i</i>, 1</sub> - <i>y</i><sub class="lower-index"><i>i</i>, 2</sub>|</span>) which are the coordinates of the opposite angles of the base of the brick number <span class="tex-span"><i>i</i></span>. The coordinates are integers and their absolute value does not exceed <span class="tex-span">50</span>. </p><p>The cubes are given in the order Vasya puts them. It is guaranteed that the area of intersection of the upper side of the brick number <span class="tex-span"><i>i</i> - 1</span> and the lower side of the brick number <span class="tex-span"><i>i</i></span> is strictly strictly greater than zero for all <span class="tex-span"><i>i</i> ≥ 2</span>.</p>

## Output

<p>Print the number of bricks in the maximal stable tower.</p>





```input1
2
0 0 3 3
1 0 4 3

```




```input2
2
0 0 3 3
2 0 5 3

```




```input3
3
0 0 3 3
1 0 4 3
2 0 5 3

```




```output1
2

```




```output2
1

```




```output3
3

```


