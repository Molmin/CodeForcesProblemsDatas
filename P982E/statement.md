## Description

<div><p>Consider a <a href="https://en.wikipedia.org/wiki/Billiard_table">billiard table</a> of rectangular size $n \times m$ with four pockets. Let's introduce a coordinate system with the origin at the lower left corner (see the picture). </p><center> <img class="tex-graphics" src="file://juj2WArc.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There is one ball at the point $(x, y)$ currently. Max comes to the table and strikes the ball. The ball starts moving along a line that is parallel to one of the axes or that makes a $45^{\circ}$ angle with them. We will assume that: </p><ol> <li> the angles between the directions of the ball before and after a collision with a side are equal, </li><li> the ball moves indefinitely long, it only stops when it falls into a pocket, </li><li> the ball can be considered as a point, it falls into a pocket if and only if its coordinates coincide with one of the pockets, </li><li> initially the ball is not in a pocket. </li></ol><p>Note that the ball can move along some side, in this case the ball will just fall into the pocket at the end of the side.</p><p>Your task is to determine whether the ball will fall into a pocket eventually, and if yes, which of the four pockets it will be.</p></div><div class="input-specification"><p>The only line contains $6$ integers $n$, $m$, $x$, $y$, $v_x$, $v_y$ ($1 \leq n, m \leq 10^9$, $0 \leq x \leq n$; $0 \leq y \leq m$; $-1 \leq v_x, v_y \leq 1$; $(v_x, v_y) \neq (0, 0)$)&nbsp;— the width of the table, the length of the table, the $x$-coordinate of the initial position of the ball, the $y$-coordinate of the initial position of the ball, the $x$-component of its initial speed and the $y$-component of its initial speed, respectively. It is guaranteed that the ball is not initially in a pocket.</p></div><div class="output-specification"><p>Print the coordinates of the pocket the ball will fall into, or $-1$ if the ball will move indefinitely.</p></div>

## Input

<p>The only line contains $6$ integers $n$, $m$, $x$, $y$, $v_x$, $v_y$ ($1 \leq n, m \leq 10^9$, $0 \leq x \leq n$; $0 \leq y \leq m$; $-1 \leq v_x, v_y \leq 1$; $(v_x, v_y) \neq (0, 0)$)&nbsp;— the width of the table, the length of the table, the $x$-coordinate of the initial position of the ball, the $y$-coordinate of the initial position of the ball, the $x$-component of its initial speed and the $y$-component of its initial speed, respectively. It is guaranteed that the ball is not initially in a pocket.</p>

## Output

<p>Print the coordinates of the pocket the ball will fall into, or $-1$ if the ball will move indefinitely.</p>





```input1
4 3 2 2 -1 1

```




```input2
4 4 2 0 1 1

```




```input3
10 10 10 1 -1 0

```




```output1
0 0
```




```output2
-1
```




```output3
-1
```



## Note

<p>The first sample: </p><center> <img class="tex-graphics" src="file://jdUDAROn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The second sample: </p><center> <img class="tex-graphics" src="file://onZ8bn0o.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third sample the ball will never change its $y$ coordinate, so the ball will never fall into a pocket.</p>
