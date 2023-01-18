## Description

<div><p>Greg the Dwarf has been really busy recently with excavations by the Neverland Mountain. However for the well-known reasons (as you probably remember he is a very unusual dwarf and he cannot stand sunlight) Greg can only excavate at night. And in the morning he should be in his crypt before the first sun ray strikes. That's why he wants to find the shortest route from the excavation point to his crypt. Greg has recollected how the Codeforces participants successfully solved the problem of transporting his coffin to a crypt. So, in some miraculous way Greg appeared in your bedroom and asks you to help him in a highly persuasive manner. As usual, you didn't feel like turning him down.</p><p>After some thought, you formalized the task as follows: as the Neverland mountain has a regular shape and ends with a rather sharp peak, it can be represented as a cone whose base radius equals <span class="tex-span"><i>r</i></span> and whose height equals <span class="tex-span"><i>h</i></span>. The graveyard where Greg is busy excavating and his crypt can be represented by two points on the cone's surface. All you've got to do is find the distance between points on the cone's surface. </p><p>The task is complicated by the fact that the mountain's base on the ground level and even everything below the mountain has been dug through by gnome (one may wonder whether they've been looking for the same stuff as Greg...). So, one can consider the shortest way to pass not only along the side surface, but also along the cone's base (and in a specific case both points can lie on the cone's base — see the first sample test)</p><p>Greg will be satisfied with the problem solution represented as the length of the shortest path between two points — he can find his way pretty well on his own. He gave you two hours to solve the problem and the time is ticking!</p></div><div class="input-specification"><p>The first input line contains space-separated integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>h</i> ≤ 1000</span>) — the base radius and the cone height correspondingly. The second and third lines contain coordinates of two points on the cone surface, groups of three space-separated real numbers. The coordinates of the points are given in the systems of coordinates where the origin of coordinates is located in the centre of the cone's base and its rotation axis matches the <span class="tex-span"><i>OZ</i></span> axis. In this coordinate system the vertex of the cone is located at the point <span class="tex-span">(0, 0, <i>h</i>)</span>, the base of the cone is a circle whose center is at the point <span class="tex-span">(0, 0, 0)</span>, lying on the <span class="tex-span"><i>XOY</i></span> plane, and all points on the cone surface have a non-negative coordinate <span class="tex-span"><i>z</i></span>. It is guaranteed that the distances from the points to the cone surface do not exceed <span class="tex-span">10<sup class="upper-index"> - 12</sup></span>. All real numbers in the input have no more than 16 digits after decimal point.</p></div><div class="output-specification"><p>Print the length of the shortest path between the points given in the input, with absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first input line contains space-separated integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>h</i> ≤ 1000</span>) — the base radius and the cone height correspondingly. The second and third lines contain coordinates of two points on the cone surface, groups of three space-separated real numbers. The coordinates of the points are given in the systems of coordinates where the origin of coordinates is located in the centre of the cone's base and its rotation axis matches the <span class="tex-span"><i>OZ</i></span> axis. In this coordinate system the vertex of the cone is located at the point <span class="tex-span">(0, 0, <i>h</i>)</span>, the base of the cone is a circle whose center is at the point <span class="tex-span">(0, 0, 0)</span>, lying on the <span class="tex-span"><i>XOY</i></span> plane, and all points on the cone surface have a non-negative coordinate <span class="tex-span"><i>z</i></span>. It is guaranteed that the distances from the points to the cone surface do not exceed <span class="tex-span">10<sup class="upper-index"> - 12</sup></span>. All real numbers in the input have no more than 16 digits after decimal point.</p>

## Output

<p>Print the length of the shortest path between the points given in the input, with absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 2
1.0 0.0 0.0
-1.0 0.0 0.0

```




```input2
2 2
1.0 0.0 0.0
1.0 0.0 1.0

```




```input3
2 2
1.0 0.0 1.0
-1.0 0.0 1.0

```




```input4
2 2
1.0 0.0 0.0
0.0 1.0 1.0

```




```output1
2.000000000
```




```output2
2.414213562
```




```output3
2.534324263
```




```output4
3.254470198
```


