## Description

<div><p><span class="tex-font-style-it">Based on a peculiar incident at basketball practice, Akari came up with the following competitive programming problem!</span></p><p>You are given $n$ points on the plane, no three of which are collinear. The $i$-th point initially has a label $a_i$, in such a way that the labels $a_1, a_2, \dots, a_n$ form a permutation of $1, 2, \dots, n$.</p><p>You are allowed to modify the labels through the following operation:</p><ol> <li> Choose two distinct integers $i$ and $j$ between $1$ and $n$. </li><li> Swap the labels of points $i$ and $j$, and finally </li><li> Draw the segment between points $i$ and $j$. </li></ol><p>A sequence of operations is valid if after applying all of the operations in the sequence in order, the $k$-th point ends up having the label $k$ for all $k$ between $1$ and $n$ inclusive, and the drawn segments don't intersect each other internally. Formally, if two of the segments intersect, then they must do so at a common endpoint of both segments.</p><p>In particular, all drawn segments must be distinct.</p><p>Find any valid sequence of operations, or say that none exist. </p></div><div class="input-specification"><p>The first line contains an integer $n$ ($3 \le n \le 2000$) &nbsp;— the number of points.</p><p>The $i$-th of the following $n$ lines contains three integers $x_i$, $y_i$, $a_i$ ($-10^6 \le x_i, y_i \le 10^6$, $1 \le a_i \le n$), representing that the $i$-th point has coordinates $(x_i, y_i)$ and initially has label $a_i$.</p><p>It is guaranteed that all points are distinct, no three points are collinear, and the labels $a_1, a_2, \dots, a_n$ form a permutation of $1, 2, \dots, n$.</p></div><div class="output-specification"><p>If it is impossible to perform a valid sequence of operations, print $-1$.</p><p>Otherwise, print an integer $k$ ($0 \le k \le \frac{n(n - 1)}{2}$) &nbsp;— the number of operations to perform, followed by $k$ lines, each containing two integers $i$ and $j$ ($1 \le i, j \le n$, $i\neq j$) &nbsp;— the indices of the points chosen for the operation.</p><p>Note that you are <span class="tex-font-style-bf">not</span> required to minimize or maximize the value of $k$.</p><p>If there are multiple possible answers, you may print any of them.</p></div>

## Input

<p>The first line contains an integer $n$ ($3 \le n \le 2000$) &nbsp;— the number of points.</p><p>The $i$-th of the following $n$ lines contains three integers $x_i$, $y_i$, $a_i$ ($-10^6 \le x_i, y_i \le 10^6$, $1 \le a_i \le n$), representing that the $i$-th point has coordinates $(x_i, y_i)$ and initially has label $a_i$.</p><p>It is guaranteed that all points are distinct, no three points are collinear, and the labels $a_1, a_2, \dots, a_n$ form a permutation of $1, 2, \dots, n$.</p>

## Output

<p>If it is impossible to perform a valid sequence of operations, print $-1$.</p><p>Otherwise, print an integer $k$ ($0 \le k \le \frac{n(n - 1)}{2}$) &nbsp;— the number of operations to perform, followed by $k$ lines, each containing two integers $i$ and $j$ ($1 \le i, j \le n$, $i\neq j$) &nbsp;— the indices of the points chosen for the operation.</p><p>Note that you are <span class="tex-font-style-bf">not</span> required to minimize or maximize the value of $k$.</p><p>If there are multiple possible answers, you may print any of them.</p>





```input1
5
-1 -2 2
3 0 5
1 3 4
4 -3 3
5 2 1
```




```input2
3
5 4 1
0 0 2
-3 -2 3
```




```output1
5
1 2
5 3
4 5
1 5
1 3
```




```output2
0
```



## Note

<p>The following animation showcases the first sample test case. The black numbers represent the indices of the points, while the boxed orange numbers represent their labels.</p><center> <img class="tex-graphics" src="file://BHpgtgjq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second test case, all labels are already in their correct positions, so no operations are necessary.</p>
