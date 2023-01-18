## Description

<div><p>You are given a set of $n$ points in a 2D plane. No three points are collinear.</p><p>A pentagram is a set of $5$ points $A,B,C,D,E$ that can be arranged as follows. <img class="tex-graphics" src="file://eX7CGFQY.png" style="max-width: 100.0%;max-height: 100.0%;"> Note the length of the line segments don't matter, only that those particular intersections exist.</p><p>Count the number of ways to choose $5$ points from the given set that form a pentagram.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($5 \leq n \leq 300$)&nbsp;— the number of points.</p><p>Each of the next $n$ lines contains two integers $x_i, y_i$ ($-10^6 \leq x_i,y_i \leq 10^6$)&nbsp;— the coordinates of the $i$-th point. It is guaranteed that no three points are collinear.</p></div><div class="output-specification"><p>Print a single integer, the number of sets of $5$ points that form a pentagram.</p></div>

## Input

<p>The first line contains an integer $n$ ($5 \leq n \leq 300$)&nbsp;— the number of points.</p><p>Each of the next $n$ lines contains two integers $x_i, y_i$ ($-10^6 \leq x_i,y_i \leq 10^6$)&nbsp;— the coordinates of the $i$-th point. It is guaranteed that no three points are collinear.</p>

## Output

<p>Print a single integer, the number of sets of $5$ points that form a pentagram.</p>





```input1
5
0 0
0 2
2 0
2 2
1 3
```




```input2
5
0 0
4 0
0 4
4 4
2 3
```




```input3
10
841746 527518
595261 331297
-946901 129987
670374 -140388
-684770 309555
-302589 415564
-387435 613331
-624940 -95922
945847 -199224
24636 -565799
```




```output1
1
```




```output2
0
```




```output3
85
```



## Note

<p>A picture of the first sample: <img class="tex-graphics" src="file://hTNBtHqP.png" style="max-width: 100.0%;max-height: 100.0%;"> A picture of the second sample: <img class="tex-graphics" src="file://1WEUYwUJ.png" style="max-width: 100.0%;max-height: 100.0%;"> A picture of the third sample: <img class="tex-graphics" src="file://OydEyaXi.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
