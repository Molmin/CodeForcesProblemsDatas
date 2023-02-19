## Description

<div><p>A running competition is going to be held soon. The stadium where the competition will be held can be represented by several segments on the coordinate plane:</p><ul> <li> two horizontal segments: one connecting the points $(0, 0)$ and $(x, 0)$, the other connecting the points $(0, y)$ and $(x, y)$; </li><li> $n + 1$ vertical segments, numbered from $0$ to $n$. The $i$-th segment connects the points $(a_i, 0)$ and $(a_i, y)$; $0 = a_0 &lt; a_1 &lt; a_2 &lt; \dots &lt; a_{n - 1} &lt; a_n = x$. </li></ul><p>For example, here is a picture of the stadium with $x = 10$, $y = 5$, $n = 3$ and $a = [0, 3, 5, 10]$:</p><center> <img class="tex-graphics" src="file://PM0d91bQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A <span class="tex-font-style-it">lap</span> is a route that goes along the segments, starts and finishes at the same point, and never intersects itself (the only two points of a lap that coincide are its starting point and ending point). The length of a lap is a total distance travelled around it. For example, the red route in the picture representing the stadium is a lap of length $24$.</p><p>The competition will be held in $q$ stages. The $i$-th stage has length $l_i$, and the organizers want to choose a lap for each stage such that the length of the lap is a <span class="tex-font-style-bf">divisor of $l_i$</span>. The organizers don't want to choose short laps for the stages, so for each stage, they want to find the maximum possible length of a suitable lap.</p><p>Help the organizers to calculate the maximum possible lengths of the laps for the stages! In other words, for every $l_i$, find the maximum possible integer $L$ such that $l_i \bmod L = 0$, and there exists a lap of length <span class="tex-font-style-bf">exactly</span> $L$.</p><p>If it is impossible to choose such a lap then print $-1$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $x$ and $y$ ($1 \le n, x, y \le 2 \cdot 10^5$, $n \le x$).</p><p>The second line contains $n + 1$ integers $a_0$, $a_1$, ..., $a_n$ ($0 = a_0 &lt; a_1 &lt; a_2 &lt; \dots &lt; a_{n - 1} &lt; a_n = x$).</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of stages.</p><p>The fourth line contains $q$ <span class="tex-font-style-bf">even</span> integers $l_1$, $l_2$, ..., $l_q$ ($4 \le l_i \le 10^6$)&nbsp;— the lengths of the stages. </p></div><div class="output-specification"><p>Print $q$ numbers. The $i$-th number should be equal to the maximum possible length of a suitable lap for the $i$-th stage, or $-1$ if it is impossible to choose a lap for that stage.</p></div>

## Input

<p>The first line contains three integers $n$, $x$ and $y$ ($1 \le n, x, y \le 2 \cdot 10^5$, $n \le x$).</p><p>The second line contains $n + 1$ integers $a_0$, $a_1$, ..., $a_n$ ($0 = a_0 &lt; a_1 &lt; a_2 &lt; \dots &lt; a_{n - 1} &lt; a_n = x$).</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of stages.</p><p>The fourth line contains $q$ <span class="tex-font-style-bf">even</span> integers $l_1$, $l_2$, ..., $l_q$ ($4 \le l_i \le 10^6$)&nbsp;— the lengths of the stages. </p>

## Output

<p>Print $q$ numbers. The $i$-th number should be equal to the maximum possible length of a suitable lap for the $i$-th stage, or $-1$ if it is impossible to choose a lap for that stage.</p>





```input1
3 10 5
0 3 5 10
6
24 30 14 16 18 10
```




```output1
24 30 14 16 -1 -1
```


