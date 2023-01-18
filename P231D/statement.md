## Description

<div><p>One day Vasya was going home when he saw a box lying on the road. The box can be represented as a rectangular parallelepiped. Vasya needed no time to realize that the box is special, as all its edges are parallel to the coordinate axes, one of its vertices is at point <span class="tex-span">(0, 0, 0)</span>, and the opposite one is at point <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>z</i><sub class="lower-index">1</sub>)</span>. The six faces of the box contain some numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">6</sub></span>, exactly one number right in the center of each face.</p><center> <img class="tex-graphics" src="file://S61dOcPT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The numbers are located on the box like that: </p><ul> <li> number <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> is written on the face that lies on the ZOX plane; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> is written on the face, parallel to the plane from the previous point; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> is written on the face that lies on the XOY plane; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> is written on the face, parallel to the plane from the previous point; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">5</sub></span> is written on the face that lies on the YOZ plane; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">6</sub></span> is written on the face, parallel to the plane from the previous point. </li></ul><p>At the moment Vasya is looking at the box from point <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span>. Find the sum of numbers that Vasya sees. Note that all faces of the box are not transparent and Vasya can't see the numbers through the box. The picture contains transparent faces just to make it easier to perceive. You can consider that if Vasya is looking from point, lying on the plane of some face, than he can not see the number that is written on this face. It is enough to see the center of a face to see the corresponding number for Vasya. Also note that Vasya always reads correctly the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> numbers that he sees, independently of their rotation, angle and other factors (that is, for example, if Vasya sees some <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 6</span>, then he can't mistake this number for <span class="tex-span">9</span> and so on). </p></div><div class="input-specification"><p>The fist input line contains three space-separated integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">|<i>x</i>|, |<i>y</i>|, |<i>z</i>| ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of Vasya's position in space. The second line contains three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>z</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of the box's vertex that is opposite to the vertex at point <span class="tex-span">(0, 0, 0)</span>. The third line contains six space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">6</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the numbers that are written on the box faces. </p><p>It is guaranteed that point <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span> is located strictly outside the box.</p></div><div class="output-specification"><p>Print a single integer — the sum of all numbers on the box faces that Vasya sees.</p></div>

## Input

<p>The fist input line contains three space-separated integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">|<i>x</i>|, |<i>y</i>|, |<i>z</i>| ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of Vasya's position in space. The second line contains three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>z</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of the box's vertex that is opposite to the vertex at point <span class="tex-span">(0, 0, 0)</span>. The third line contains six space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">6</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the numbers that are written on the box faces. </p><p>It is guaranteed that point <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span> is located strictly outside the box.</p>

## Output

<p>Print a single integer — the sum of all numbers on the box faces that Vasya sees.</p>





```input1
2 2 2
1 1 1
1 2 3 4 5 6

```




```input2
0 0 10
3 2 3
1 2 3 4 5 6

```




```output1
12

```




```output2
4

```



## Note

<p>The first sample corresponds to perspective, depicted on the picture. Vasya sees numbers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> (on the top face that is the darkest), <span class="tex-span"><i>a</i><sub class="lower-index">6</sub></span> (on the right face that is the lightest) and <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> (on the left visible face).</p><p>In the second sample Vasya can only see number <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span>.</p>
