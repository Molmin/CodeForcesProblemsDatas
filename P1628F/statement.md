## Description

<div><p><span class="tex-font-style-it">NASA (Norwegian Astronaut Stuff Association) is developing a new steering system for spaceships. But in its current state, it wouldn't be very safe if the spaceship would end up in a bunch of space junk. To make the steering system safe, they need to answer the following:</span></p><p>Given the target position $t = (0, 0)$, a set of $n$ pieces of space junk $l$ described by line segments $l_i = ((a_{ix}, a_{iy}), (b_{ix}, b_{iy}))$, and a starting position $s = (s_x, s_y)$, is there a direction such that floating in that direction from the starting position would lead to the target position?</p><p>When the spaceship hits a piece of space junk, what happens depends on the absolute difference in angle between the floating direction and the line segment, $\theta$:</p><ul> <li> If $\theta &lt; 45^{\circ}$, the spaceship slides along the piece of space junk in the direction that minimizes the change in angle, and when the spaceship slides off the end of the space junk, it continues floating in the direction it came in (before hitting the space junk). </li><li> If $\theta \ge 45^{\circ}$, the spaceship stops, because there is too much friction to slide along the space junk. </li></ul><p>You are only given the set of pieces of space junk once, and the target position is always $(0, 0)$, but there are $q$ queries, each with a starting position $s_j = (s_{jx}, s_{jy})$.</p><p>Answer the above question for each query.</p></div><div class="input-specification"><p>The first line contains the the integer $n$ ($1 \le n \le 1500$).</p><p>Then follows $n$ lines, the $i$-th of which containing the $4$ integers $a_{ix}$, $a_{iy}$, $b_{ix}$, and $b_{iy}$ ($|a_{ix}|, |a_{iy}|, |b_{ix}|, |b_{iy}| \le 1000$).</p><p>Then follows a line containing the integer $q$ ($1 \le q \le 1000$).</p><p>Then follows $q$ lines, the $j$-th of which containing the $2$ integers $s_{jx}$ and $s_{jy}$ ($|s_{jx}|, |s_{jy}| \le 1000$).</p><p>It is guaranteed that none of the segments in $l$ cross or touch, that $t$ is not on any segment in $l$, that $s_j$ is not on any segment in $l$, and that $s \neq t$.</p></div><div class="output-specification"><p>For each query $s_j$ print an answer. If there exists a direction such that floating from $s_j$ in that direction, possibly sliding along some pieces of space junk, leads to $t$, print "YES". Otherwise, print "NO" (case insensitive).</p></div>

## Input

<p>The first line contains the the integer $n$ ($1 \le n \le 1500$).</p><p>Then follows $n$ lines, the $i$-th of which containing the $4$ integers $a_{ix}$, $a_{iy}$, $b_{ix}$, and $b_{iy}$ ($|a_{ix}|, |a_{iy}|, |b_{ix}|, |b_{iy}| \le 1000$).</p><p>Then follows a line containing the integer $q$ ($1 \le q \le 1000$).</p><p>Then follows $q$ lines, the $j$-th of which containing the $2$ integers $s_{jx}$ and $s_{jy}$ ($|s_{jx}|, |s_{jy}| \le 1000$).</p><p>It is guaranteed that none of the segments in $l$ cross or touch, that $t$ is not on any segment in $l$, that $s_j$ is not on any segment in $l$, and that $s \neq t$.</p>

## Output

<p>For each query $s_j$ print an answer. If there exists a direction such that floating from $s_j$ in that direction, possibly sliding along some pieces of space junk, leads to $t$, print "YES". Otherwise, print "NO" (case insensitive).</p>





```input1
3
0 1 2 4
1 3 -1 6
0 -1 1 -1
14
-2 10
-1 10
0 10
1 10
2 10
3 10
4 10
5 10
6 10
-1 -2
0 -2
1 -2
2 -2
3 -2
```




```output1
YES
YES
YES
YES
YES
NO
NO
NO
YES
YES
NO
NO
NO
YES
```



## Note

<p><img class="tex-graphics" src="file://nSig6wWb.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"></p><p>The blue cross represents the target location, and the other blue line segments represent the space junk.</p><p>Green dots represent starting locations where the answer is yes, and red dots represent starting locations where the answer is no.</p><p>The yellow lines are possible paths to the target location for the $3$rd and $14$th queries. </p><p>The black line is a possible path from the starting location in the $6$th query, but it barely misses the target location.</p>
