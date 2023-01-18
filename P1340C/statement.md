## Description

<div><p><span class="tex-font-style-it"> If the girl doesn't go to Denis, then Denis will go to the girl. Using this rule, the young man left home, bought flowers and went to Nastya. </span></p><p>On the way from Denis's house to the girl's house is a road of $n$ lines. This road can't be always crossed in one green light. Foreseeing this, the good mayor decided to place safety islands in some parts of the road. Each safety island is located after a line, as well as at the beginning and at the end of the road. Pedestrians can relax on them, gain strength and wait for a green light.</p><p>Denis came to the edge of the road exactly at the moment when the green light turned on. The boy knows that the traffic light first lights up $g$ seconds green, and then $r$ seconds red, then again $g$ seconds green and so on.</p><p>Formally, the road can be represented as a segment $[0, n]$. Initially, Denis is at point $0$. His task is to get to point $n$ in the shortest possible time.</p><p>He knows many different integers $d_1, d_2, \ldots, d_m$, where $0 \leq d_i \leq n$ &nbsp;— are the coordinates of points, in which the safety islands are located. Only at one of these points, the boy can be at a time when the red light is on.</p><p>Unfortunately, Denis isn't always able to control himself because of the excitement, so some restrictions are imposed:</p><ul> <li> He must always move while the green light is on because it's difficult to stand when so beautiful girl is waiting for you. Denis can change his position by $\pm 1$ in $1$ second. While doing so, he must always stay inside the segment $[0, n]$. </li><li> He can change his direction only on the safety islands (because it is safe). This means that if in the previous second the boy changed his position by $+1$ and he walked on a safety island, then he can change his position by $\pm 1$. Otherwise, he can change his position only by $+1$. Similarly, if in the previous second he changed his position by $-1$, on a safety island he can change position by $\pm 1$, and at any other point by $-1$. </li><li> At the moment when the red light is on, the boy must be on one of the safety islands. He can continue moving in any direction when the green light is on. </li></ul><p>Denis has crossed the road as soon as his coordinate becomes equal to $n$.</p><p>This task was not so simple, because it's possible that it is impossible to cross the road. Since Denis has all thoughts about his love, he couldn't solve this problem and asked us to help him. Find the minimal possible time for which he can cross the road according to these rules, or find that it is impossible to do.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ $(1 \leq n \leq 10^6, 2 \leq m \leq min(n + 1, 10^4))$ &nbsp;— road width and the number of safety islands.</p><p>The second line contains $m$ distinct integers $d_1, d_2, \ldots, d_m$ $(0 \leq d_i \leq n)$ &nbsp;— the points where the safety islands are located. It is guaranteed that there are $0$ and $n$ among them.</p><p>The third line contains two integers $g, r$ $(1 \leq g, r \leq 1000)$ &nbsp;— the time that the green light stays on and the time that the red light stays on.</p></div><div class="output-specification"><p>Output a single integer &nbsp;— the minimum time for which Denis can cross the road with obeying all the rules.</p><p>If it is impossible to cross the road output $-1$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ $(1 \leq n \leq 10^6, 2 \leq m \leq min(n + 1, 10^4))$ &nbsp;— road width and the number of safety islands.</p><p>The second line contains $m$ distinct integers $d_1, d_2, \ldots, d_m$ $(0 \leq d_i \leq n)$ &nbsp;— the points where the safety islands are located. It is guaranteed that there are $0$ and $n$ among them.</p><p>The third line contains two integers $g, r$ $(1 \leq g, r \leq 1000)$ &nbsp;— the time that the green light stays on and the time that the red light stays on.</p>

## Output

<p>Output a single integer &nbsp;— the minimum time for which Denis can cross the road with obeying all the rules.</p><p>If it is impossible to cross the road output $-1$.</p>





```input1
15 5
0 3 7 14 15
11 11
```




```input2
13 4
0 3 7 13
9 9
```




```output1
45
```




```output2
-1
```



## Note

<p>In the first test, the optimal route is: </p><ul> &nbsp;&nbsp;&nbsp;&nbsp;<li> for the first green light, go to $7$ and return to $3$. In this case, we will change the direction of movement at the point $7$, which is allowed, since there is a safety island at this point. In the end, we will be at the point of $3$, where there is also a safety island. The next $11$ seconds we have to wait for the red light. &nbsp;&nbsp;&nbsp;&nbsp;</li><li> for the second green light reaches $14$. Wait for the red light again. &nbsp;&nbsp;&nbsp;&nbsp;</li><li> for $1$ second go to $15$. As a result, Denis is at the end of the road. </li></ul><p>In total, $45$ seconds are obtained.</p><p>In the second test, it is impossible to cross the road according to all the rules.</p>
