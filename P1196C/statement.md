## Description

<div><p>$n$ robots have escaped from your laboratory! You have to find them as soon as possible, because these robots are experimental, and their behavior is not tested yet, so they may be really dangerous!</p><p>Fortunately, even though your robots have escaped, you still have some control over them. First of all, you know the location of each robot: the world you live in can be modeled as an infinite coordinate plane, and the $i$-th robot is currently located at the point having coordinates ($x_i$, $y_i$). Furthermore, you may send exactly one command to all of the robots. The command should contain two integer numbers $X$ and $Y$, and when each robot receives this command, it starts moving towards the point having coordinates ($X$, $Y$). The robot stops its movement in two cases:</p><ul> <li> either it reaches ($X$, $Y$); </li><li> or it cannot get any closer to ($X$, $Y$). </li></ul><p>Normally, all robots should be able to get from any point of the coordinate plane to any other point. Each robot usually can perform four actions to move. Let's denote the current coordinates of the robot as ($x_c$, $y_c$). Then the movement system allows it to move to any of the four adjacent points:</p><ol> <li> the first action allows it to move from ($x_c$, $y_c$) to ($x_c - 1$, $y_c$); </li><li> the second action allows it to move from ($x_c$, $y_c$) to ($x_c$, $y_c + 1$); </li><li> the third action allows it to move from ($x_c$, $y_c$) to ($x_c + 1$, $y_c$); </li><li> the fourth action allows it to move from ($x_c$, $y_c$) to ($x_c$, $y_c - 1$). </li></ol><p>Unfortunately, it seems that some movement systems of some robots are malfunctioning. For each robot you know which actions it can perform, and which it cannot perform.</p><p>You want to send a command so all robots gather at the same point. To do so, you have to choose a pair of integer numbers $X$ and $Y$ so that each robot can reach the point ($X$, $Y$). Is it possible to find such a point?</p></div><div class="input-specification"><p>The first line contains one integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>Then $q$ queries follow. Each query begins with one line containing one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of robots in the query. Then $n$ lines follow, the $i$-th of these lines describes the $i$-th robot in the current query: it contains six integer numbers $x_i$, $y_i$, $f_{i, 1}$, $f_{i, 2}$, $f_{i, 3}$ and $f_{i, 4}$ ($-10^5 \le x_i, y_i \le 10^5$, $0 \le f_{i, j} \le 1$). The first two numbers describe the initial location of the $i$-th robot, and the following four numbers describe which actions the $i$-th robot can use to move ($f_{i, j} = 1$ if the $i$-th robot can use the $j$-th action, and $f_{i, j} = 0$ if it cannot use the $j$-th action).</p><p>It is guaranteed that the total number of robots over all queries does not exceed $10^5$.</p></div><div class="output-specification"><p>You should answer each query independently, in the order these queries appear in the input.</p><p>To answer a query, you should do one of the following:</p><ul> <li> if it is impossible to find a point that is reachable by all $n$ robots, print one number $0$ on a separate line; </li><li> if it is possible to find a point that is reachable by all $n$ robots, print three space-separated integers on the same line: $1$ $X$ $Y$, where $X$ and $Y$ are the coordinates of the point reachable by all $n$ robots. <span class="tex-font-style-it">Both $X$ and $Y$ should not exceed $10^5$ by absolute value; it is guaranteed that if there exists at least one point reachable by all robots, then at least one of such points has both coordinates not exceeding $10^5$ by absolute value</span>.</li></ul></div>

## Input

<p>The first line contains one integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>Then $q$ queries follow. Each query begins with one line containing one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of robots in the query. Then $n$ lines follow, the $i$-th of these lines describes the $i$-th robot in the current query: it contains six integer numbers $x_i$, $y_i$, $f_{i, 1}$, $f_{i, 2}$, $f_{i, 3}$ and $f_{i, 4}$ ($-10^5 \le x_i, y_i \le 10^5$, $0 \le f_{i, j} \le 1$). The first two numbers describe the initial location of the $i$-th robot, and the following four numbers describe which actions the $i$-th robot can use to move ($f_{i, j} = 1$ if the $i$-th robot can use the $j$-th action, and $f_{i, j} = 0$ if it cannot use the $j$-th action).</p><p>It is guaranteed that the total number of robots over all queries does not exceed $10^5$.</p>

## Output

<p>You should answer each query independently, in the order these queries appear in the input.</p><p>To answer a query, you should do one of the following:</p><ul> <li> if it is impossible to find a point that is reachable by all $n$ robots, print one number $0$ on a separate line; </li><li> if it is possible to find a point that is reachable by all $n$ robots, print three space-separated integers on the same line: $1$ $X$ $Y$, where $X$ and $Y$ are the coordinates of the point reachable by all $n$ robots. <span class="tex-font-style-it">Both $X$ and $Y$ should not exceed $10^5$ by absolute value; it is guaranteed that if there exists at least one point reachable by all robots, then at least one of such points has both coordinates not exceeding $10^5$ by absolute value</span>.</li></ul>





```input1
4
2
-1 -2 0 0 0 0
-1 -2 0 0 0 0
3
1 5 1 1 1 1
2 5 0 1 0 1
3 5 1 0 0 0
2
1337 1337 0 1 1 1
1336 1337 1 1 0 1
1
3 5 1 1 1 1
```




```output1
1 -1 -2
1 2 5
0
1 -100000 -100000
```


