## Description

<div><p>Let's denote the Manhattan distance between two points $p_1$ (with coordinates $(x_1, y_1)$) and $p_2$ (with coordinates $(x_2, y_2)$) as $d(p_1, p_2) = |x_1 - x_2| + |y_1 - y_2|$. For example, the distance between two points with coordinates $(1, 3)$ and $(4, 2)$ is $|1 - 4| + |3 - 2| = 4$.</p><p>You are given two points, $A$ and $B$. The point $A$ has coordinates $(0, 0)$, the point $B$ has coordinates $(x, y)$.</p><p>Your goal is to find a point $C$ such that:</p><ul> <li> both coordinates of $C$ are non-negative integers; </li><li> $d(A, C) = \dfrac{d(A, B)}{2}$ (without any rounding); </li><li> $d(B, C) = \dfrac{d(A, B)}{2}$ (without any rounding). </li></ul><p>Find any point $C$ that meets these constraints, or report that no such point exists.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 3000$) — the number of test cases.</p><p>Each test case consists of one line containing two integers $x$ and $y$ ($0 \le x, y \le 50$) — the coordinates of the point $B$.</p></div><div class="output-specification"><p>For each test case, print the answer on a separate line as follows:</p><ul> <li> if it is impossible to find a point $C$ meeting the constraints, print "<span class="tex-font-style-tt">-1 -1</span>" (without quotes); </li><li> otherwise, print two non-negative integers not exceeding $10^6$ — the coordinates of point $C$ meeting the constraints. If there are multiple answers, print any of them. It can be shown that if any such point exists, it's possible to find a point with coordinates not exceeding $10^6$ that meets the constraints. </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 3000$) — the number of test cases.</p><p>Each test case consists of one line containing two integers $x$ and $y$ ($0 \le x, y \le 50$) — the coordinates of the point $B$.</p>

## Output

<p>For each test case, print the answer on a separate line as follows:</p><ul> <li> if it is impossible to find a point $C$ meeting the constraints, print "<span class="tex-font-style-tt">-1 -1</span>" (without quotes); </li><li> otherwise, print two non-negative integers not exceeding $10^6$ — the coordinates of point $C$ meeting the constraints. If there are multiple answers, print any of them. It can be shown that if any such point exists, it's possible to find a point with coordinates not exceeding $10^6$ that meets the constraints. </li></ul>





```input1
10
49 3
2 50
13 0
0 41
42 0
0 36
13 37
42 16
42 13
0 0
```




```output1
23 3
1 25
-1 -1
-1 -1
21 0
0 18
13 12
25 4
-1 -1
0 0
```



## Note

<p>Explanations for some of the test cases from the example:</p><ul> <li> In the first test case, the point $B$ has coordinates $(49, 3)$. If the point $C$ has coordinates $(23, 3)$, then the distance from $A$ to $B$ is $|49 - 0| + |3 - 0| = 52$, the distance from $A$ to $C$ is $|23 - 0| + |3 - 0| = 26$, and the distance from $B$ to $C$ is $|23 - 49| + |3 - 3| = 26$. </li><li> In the second test case, the point $B$ has coordinates $(2, 50)$. If the point $C$ has coordinates $(1, 25)$, then the distance from $A$ to $B$ is $|2 - 0| + |50 - 0| = 52$, the distance from $A$ to $C$ is $|1 - 0| + |25 - 0| = 26$, and the distance from $B$ to $C$ is $|1 - 2| + |25 - 50| = 26$. </li><li> In the third and the fourth test cases, it can be shown that no point with integer coordinates meets the constraints. </li><li> In the fifth test case, the point $B$ has coordinates $(42, 0)$. If the point $C$ has coordinates $(21, 0)$, then the distance from $A$ to $B$ is $|42 - 0| + |0 - 0| = 42$, the distance from $A$ to $C$ is $|21 - 0| + |0 - 0| = 21$, and the distance from $B$ to $C$ is $|21 - 42| + |0 - 0| = 21$. </li></ul>
