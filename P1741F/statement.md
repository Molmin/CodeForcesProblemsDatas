## Description

<div><p>Dmitry has $n$ segments of different colors on the coordinate axis $Ox$. Each segment is characterized by three integers $l_i$, $r_i$ and $c_i$ ($1 \le l_i \le r_i \le 10^9, 1 \le c_i \le n$), where $l_i$ and $r_i$ are are the coordinates of the ends of the $i$-th segment, and $c_i$ is its color.</p><p>Dmitry likes to find the minimum distances between segments. However, he considers pairs of segments of the same color uninteresting. Therefore, he wants to know for each segment the distance from this segment to the nearest <span class="tex-font-style-bf">differently</span> colored segment.</p><p>The distance between two segments is the minimum of the distances between a point of the first segment and a point of the second segment. In particular, if the segments intersect, then the distance between them is equal to $0$.</p><p>For example, Dmitry has $5$ segments:</p><center> <img class="tex-graphics" src="file://HdlhE7R3.png" style="max-width: 100.0%;max-height: 100.0%;">  </center><ul> <li> The first segment intersects with the second (and these are segments of different colors), so the answers for them are equal to $0$. </li><li> For the $3$-rd segment, the nearest segment of a different color is the $2$-nd segment, the distance to which is equal to $2$. </li><li> For the $4$-th segment, the nearest segment of a different color is the $5$-th segment, the distance to which is equal to $1$. </li><li> The $5$-th segment lies inside the $2$-nd segment (and these are segments of different colors), so the answers for them are equal to $0$. </li></ul></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of description of each test case contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of segments.</p><p>The next $n$ lines contain descriptions of the segments. Each segment is described by three integers $l_i$, $r_i$ and $c_i$ ($1 \le l_i \le r_i \le 10^9, 1 \le c_i \le n$) — coordinates of the left and right ends of $i$-th segment, as well as the color of this segment. It is guaranteed that there are at least $2$ segments of different colors.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, on a separate line print $n$ integers, where the $i$-th number is equal to the distance from the $i$-th segment to the nearest segment of a different color.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of description of each test case contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of segments.</p><p>The next $n$ lines contain descriptions of the segments. Each segment is described by three integers $l_i$, $r_i$ and $c_i$ ($1 \le l_i \le r_i \le 10^9, 1 \le c_i \le n$) — coordinates of the left and right ends of $i$-th segment, as well as the color of this segment. It is guaranteed that there are at least $2$ segments of different colors.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, on a separate line print $n$ integers, where the $i$-th number is equal to the distance from the $i$-th segment to the nearest segment of a different color.</p>





```input1|2,3,4,5,9,10,11,12,13,14,21,22,23,28,29,30,31,39,40,41
9
3
1 2 1
3 4 1
5 6 2
2
100000000 200000000 1
900000000 1000000000 2
5
1 2 1
2 3 2
3 4 3
4 5 4
5 6 5
5
1 5 1
4 9 2
1 2 1
8 9 2
5 7 3
2
1 100 2
10 90 1
3
1 1 1
10 10 2
1000000000 1000000000 3
3
3 4 1
2 5 1
1 6 2
6
5 6 2
11 12 3
7 8 2
3 4 2
1 2 1
9 10 2
2
1 3 1
2 3 2
```




```input2|2,3,4,5,6,7,8,9,10,21,22,23,24,25,26,27,28,29,30
4
8
11 16 7
12 15 7
2 5 8
17 22 5
1 8 8
19 23 8
16 16 6
6 7 5
9
1 4 3
5 11 1
8 11 3
1 10 1
2 11 1
1 10 4
3 11 1
5 7 1
1 11 1
9
25 25 1
26 26 1
24 24 2
13 14 2
12 16 2
17 18 1
19 19 1
24 27 2
24 27 1
9
15 18 1
20 22 2
13 22 2
13 22 2
3 13 2
6 10 2
3 6 2
19 24 2
22 24 2
```




```output1
3 1 1 
700000000 700000000 
0 0 0 0 0 
0 0 2 1 0 
0 0 
9 9 999999990 
0 0 0 
3 1 3 1 1 1 
0 0
```




```output2
0 1 1 0 0 0 0 0 
0 0 0 0 0 0 0 0 0 
0 0 0 3 1 1 3 0 0 
0 2 0 0 2 5 9 1 4
```



## Note

<p>In the first test case of the first sample there is only one segment of color $2$, and all other segments have color $1$. Therefore, for segments of color $1$, the answer is equal to the distance to the $3$rd segment, and for $3$rd one, the answer is equal to the minimum of the distances to segments of color $1$.</p><p>In the second test case of the first sample there are only $2$ segments, and for both of them the answer is equal to the distance between them.</p><p>In the third test case of the first sample, each segment intersects at least one of its ends with a segment of a different color, so all answers are equal to $0$.</p><p>The fourth test case of the first sample is described in the problem statement.</p><p>In the fifth test case of the first sample, one segment lies completely inside the other, and for both of them the answer is $0$.</p><p>In the sixth test case of the first sample, all segments are points of different colors.</p>
