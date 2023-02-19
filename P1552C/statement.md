## Description

<div><p>On a circle lie $2n$ distinct points, with the following property: however you choose $3$ chords that connect $3$ disjoint pairs of points, no point strictly inside the circle belongs to all $3$ chords. The points are numbered $1, \, 2, \, \dots, \, 2n$ in clockwise order.</p><p>Initially, $k$ chords connect $k$ pairs of points, in such a way that all the $2k$ endpoints of these chords are distinct.</p><p>You want to draw $n - k$ additional chords that connect the remaining $2(n - k)$ points (each point must be an endpoint of exactly one chord).</p><p>In the end, let $x$ be the total number of intersections among all $n$ chords. Compute the maximum value that $x$ can attain if you choose the $n - k$ chords optimally.</p><p>Note that the exact position of the $2n$ points is not relevant, as long as the property stated in the first paragraph holds.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 100$, $0 \le k \le n$) — half the number of points and the number of chords initially drawn.</p><p>Then $k$ lines follow. The $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i, \, y_i \le 2n$, $x_i \ne y_i$) — the endpoints of the $i$-th chord. It is guaranteed that the $2k$ numbers $x_1, \, y_1, \, x_2, \, y_2, \, \dots, \, x_k, \, y_k$ are all distinct.</p></div><div class="output-specification"><p>For each test case, output the maximum number of intersections that can be obtained by drawing $n - k$ additional chords.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 100$, $0 \le k \le n$) — half the number of points and the number of chords initially drawn.</p><p>Then $k$ lines follow. The $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i, \, y_i \le 2n$, $x_i \ne y_i$) — the endpoints of the $i$-th chord. It is guaranteed that the $2k$ numbers $x_1, \, y_1, \, x_2, \, y_2, \, \dots, \, x_k, \, y_k$ are all distinct.</p>

## Output

<p>For each test case, output the maximum number of intersections that can be obtained by drawing $n - k$ additional chords.</p>





```input1
4
4 2
8 2
1 5
1 1
2 1
2 0
10 6
14 6
2 20
9 10
13 18
15 12
11 7
```




```output1
4
0
1
14
```



## Note

<p>In the <span class="tex-font-style-bf">first test case</span>, there are three ways to draw the $2$ additional chords, shown below (black chords are the ones initially drawn, while red chords are the new ones):</p><center> <img class="tex-graphics" src="file://5C3OIAl7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>We see that the third way gives the maximum number of intersections, namely $4$.</p><p>In the <span class="tex-font-style-bf">second test case</span>, there are no more chords to draw. Of course, with only one chord present there are no intersections.</p><p>In the <span class="tex-font-style-bf">third test case</span>, we can make at most one intersection by drawing chords $1-3$ and $2-4$, as shown below:</p><center> <img class="tex-graphics" src="file://jK0UaPJz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
