## Description

<div><p>Little girl Masha likes winter sports, today she's planning to take part in slalom skiing.</p><p>The track is represented as a grid composed of <span class="tex-span"><i>n</i> × <i>m</i></span> squares. There are rectangular obstacles at the track, composed of grid squares. Masha must get from the square <span class="tex-span">(1, 1)</span> to the square <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. She can move from a square to adjacent square: either to the right, or upwards. If the square is occupied by an obstacle, it is not allowed to move to that square.</p><p>One can see that each obstacle can actually be passed in two ways: either it is to the right of Masha's path, or to the left. Masha likes to try all ways to do things, so she would like to know how many ways are there to pass the track. Two ways are considered different if there is an obstacle such that it is to the right of the path in one way, and to the left of the path in the other way.</p><p>Help Masha to find the number of ways to pass the track. The number of ways can be quite big, so Masha would like to know it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>The pictures below show different ways to pass the track in sample tests. <img class="tex-graphics" src="file://8H7XBSEx.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://CsB3lNVs.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://AGs25TxJ.png" style="max-width: 100.0%;max-height: 100.0%;"></p></div><div class="input-specification"><p>The first line of input data contains three positive integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the size of the track and the number of obstacles.</p><p>The following <span class="tex-span"><i>k</i></span> lines contain four positive integers each: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>)&nbsp;— coordinates of bottom left, and top right squares of the obstacle. </p><p>It is guaranteed that there are no obstacles at squares <span class="tex-span">(1, 1)</span> and <span class="tex-span">(<i>n</i>, <i>m</i>)</span>, and no obstacles overlap (but some of them may touch).</p></div><div class="output-specification"><p>Output one integer&nbsp;— the number of ways to pass the track modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input data contains three positive integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the size of the track and the number of obstacles.</p><p>The following <span class="tex-span"><i>k</i></span> lines contain four positive integers each: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>)&nbsp;— coordinates of bottom left, and top right squares of the obstacle. </p><p>It is guaranteed that there are no obstacles at squares <span class="tex-span">(1, 1)</span> and <span class="tex-span">(<i>n</i>, <i>m</i>)</span>, and no obstacles overlap (but some of them may touch).</p>

## Output

<p>Output one integer&nbsp;— the number of ways to pass the track modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 3 0

```




```input2
4 5 1
2 2 3 4

```




```input3
5 5 3
2 2 2 3
4 2 5 2
4 4 4 4

```




```output1
1

```




```output2
2

```




```output3
3

```


