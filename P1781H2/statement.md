## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. In this version, the constraints on $h$ and $w$ are higher.</span></p><p>A house at the sea has $h$ floors, all of the same height. The side of the house facing the sea has $w$ windows at equal distances from each other on every floor. Thus, the windows are positioned in cells of a rectangular grid of size $h \times w$.</p><p>In every window, the light can be turned either on or off, except for the given $k$ (at most $2$) windows. In these $k$ windows the light can not be turned on, because it is broken.</p><p>In the dark, we can send a signal to a ship at sea using a configuration of lights turned on and off. However, the ship can not see the position of the lights with respect to the house. Thus, if one configuration of windows with lights on can be transformed into another using parallel translation, these configurations are considered equal. Note that only parallel translation is allowed, but neither rotations nor flips are. Moreover, a configuration without any light at all is not considered valid.</p><p>Find how many different signals the ship can receive and print this number modulo $998\,244\,353$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $h$, $w$, and $k$&nbsp;($1 \le h, w \le 200$; $0 \le k \le \min(h \cdot w, 2)$)&nbsp;— the height of the house, the number of windows on each floor, and the number of windows with broken lights.</p><p>If $k &gt; 0$, each of the next $k$ lines contains two integers $r_i$ and $c_i$&nbsp;($1 \le r_i \le h$; $1 \le c_i \le w$)&nbsp;— the floor number and the window number with the broken light. The floors are numbered $1$ to $h$ from bottom to top, and the windows are numbered $1$ to $w$ from left to right. If $k = 2$, then either $r_1 \ne r_2$ or $c_1 \ne c_2$.</p><p>It is guaranteed that the sum of $h \cdot w$ over all test cases does not exceed $40\,000$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the number of signals the ship can receive, modulo $998\,244\,353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $h$, $w$, and $k$&nbsp;($1 \le h, w \le 200$; $0 \le k \le \min(h \cdot w, 2)$)&nbsp;— the height of the house, the number of windows on each floor, and the number of windows with broken lights.</p><p>If $k &gt; 0$, each of the next $k$ lines contains two integers $r_i$ and $c_i$&nbsp;($1 \le r_i \le h$; $1 \le c_i \le w$)&nbsp;— the floor number and the window number with the broken light. The floors are numbered $1$ to $h$ from bottom to top, and the windows are numbered $1$ to $w$ from left to right. If $k = 2$, then either $r_1 \ne r_2$ or $c_1 \ne c_2$.</p><p>It is guaranteed that the sum of $h \cdot w$ over all test cases does not exceed $40\,000$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the number of signals the ship can receive, modulo $998\,244\,353$.</p>





```input1|2,4,6,9,10,13,14,15
10
1 3 0
2 2 0
3 2 0
4 5 0
12 7 0
1 1 1
1 1
1 3 1
1 2
3 4 1
3 4
2 3 2
1 1
2 1
4 5 2
2 3
4 2
```




```output1
4
10
44
954368
34903934
0
2
1696
10
253144
```



## Note

<p>In the first test case, the ship can receive four different signals: all lights on; lights on in two neighboring windows; lights on in the leftmost and the rightmost windows; or light on in any single window.</p>
