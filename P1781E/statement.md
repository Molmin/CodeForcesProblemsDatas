## Description

<div><p>You have a rectangular grid of height $2$ and width $10^9$ consisting of unit cells. There are $n$ rectangles placed on this grid, and the borders of these rectangles pass along cell borders. The $i$-th rectangle covers all cells in rows from $u_i$ to $d_i$ inclusive and columns from $l_i$ to $r_i$ inclusive ($1 \le u_i \le d_i \le 2$; $1 \le l_i \le r_i \le 10^9$). The initial rectangles can intersect, be nested, and coincide arbitrarily.</p><p>You should either remove each rectangle, or replace it with any of its non-empty subrectangles. In the latter case, the new subrectangle must lie inside the initial rectangle, and its borders must still pass along cell borders. In particular, it is allowed for the subrectangle to be equal to the initial rectangle.</p><p>After that replacement, no two (non-removed) rectangles are allowed to have common cells, and the total area covered with the new rectangles must be as large as possible.</p><center> <img class="tex-graphics" src="file://wVOmZhnl.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"> <span class="tex-font-size-small">Illustration for the first test case. The initial rectangles are given at the top, the new rectangles are given at the bottom. Rectangle number $4$ is removed.</span> </center></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$&nbsp;($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of rectangles.</p><p>Each of the next $n$ lines contains four integers $u_i, l_i, d_i, r_i$&nbsp;($1 \le u_i \le d_i \le 2$; $1 \le l_i \le r_i \le 10^9$)&nbsp;— the coordinates of cells located in the top-left and the bottom-right corners of the rectangle, respectively.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, first print an integer $s$&nbsp;— the largest possible covered by new rectangles area. Then print $n$ lines with your solution to cover this area.</p><p>In the $i$-th of these lines print four integers $u'_i, l'_i, d'_i, r'_i$. If you remove the $i$-th rectangle, print $u'_i = l'_i = d'_i = r'_i = 0$. Otherwise, these numbers denote the new coordinates of the top-left and the bottom-right corners of the $i$-th rectangle, satisfying $u_i \le u'_i \le d'_i \le d_i$; $l_i \le l'_i \le r'_i \le r_i$.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$&nbsp;($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of rectangles.</p><p>Each of the next $n$ lines contains four integers $u_i, l_i, d_i, r_i$&nbsp;($1 \le u_i \le d_i \le 2$; $1 \le l_i \le r_i \le 10^9$)&nbsp;— the coordinates of cells located in the top-left and the bottom-right corners of the rectangle, respectively.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, first print an integer $s$&nbsp;— the largest possible covered by new rectangles area. Then print $n$ lines with your solution to cover this area.</p><p>In the $i$-th of these lines print four integers $u'_i, l'_i, d'_i, r'_i$. If you remove the $i$-th rectangle, print $u'_i = l'_i = d'_i = r'_i = 0$. Otherwise, these numbers denote the new coordinates of the top-left and the bottom-right corners of the $i$-th rectangle, satisfying $u_i \le u'_i \le d'_i \le d_i$; $l_i \le l'_i \le r'_i \le r_i$.</p><p>If there are multiple solutions, print any.</p>





```input1|2,3,4,5,6,7,11,12,13,20,21,22,26,27,28
8
5
1 2 2 4
2 4 2 8
1 4 2 7
1 2 1 2
1 9 1 10
2
1 1 1 10
1 5 1 15
2
1 1 1 10
1 1 1 10
5
1 3 1 7
1 3 1 8
1 1 1 4
1 2 1 7
1 10 1 11
2
1 1 2 10
1 5 1 8
2
1 5 2 10
1 2 1 7
2
1 5 2 10
2 2 2 15
5
2 6 2 7
1 4 2 5
1 5 1 9
1 7 2 10
1 2 1 6
```




```output1
15
1 2 2 4
2 5 2 8
1 5 1 7
0 0 0 0
1 9 1 10
15
1 1 1 10
1 11 1 15
10
1 1 1 10
0 0 0 0
10
0 0 0 0
1 8 1 8
1 1 1 4
1 5 1 7
1 10 1 11
20
1 1 2 10
0 0 0 0
15
1 5 2 10
1 2 1 4
20
1 5 1 10
2 2 2 15
16
2 6 2 6
2 4 2 5
0 0 0 0
1 7 2 10
1 2 1 6
```



## Note

<p>The picture in the statement illustrates the first test case.</p>
