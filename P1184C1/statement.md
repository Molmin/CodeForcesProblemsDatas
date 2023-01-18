## Description

<div><p>The Cybermen and the Daleks have long been the Doctor's main enemies. Everyone knows that both these species enjoy destroying everything they encounter. However, a little-known fact about them is that they both also love taking Turing tests!</p><p>Heidi designed a series of increasingly difficult tasks for them to spend their time on, which would allow the Doctor enough time to save innocent lives!</p><p>The funny part is that these tasks would be very easy for a human to solve.</p><p>The first task is as follows. There are some points on the plane. All but one of them are on the boundary of an axis-aligned square (its sides are parallel to the axes). Identify that point.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \le n \le 10$).</p><p>Each of the following $4n + 1$ lines contains two integers $x_i, y_i$ ($0 \leq x_i, y_i \leq 50$), describing the coordinates of the next point.</p><p>It is guaranteed that there are at least $n$ points on each side of the square and all $4n + 1$ points are distinct.</p></div><div class="output-specification"><p>Print two integers&nbsp;— the coordinates of the point that is not on the boundary of the square.</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \le n \le 10$).</p><p>Each of the following $4n + 1$ lines contains two integers $x_i, y_i$ ($0 \leq x_i, y_i \leq 50$), describing the coordinates of the next point.</p><p>It is guaranteed that there are at least $n$ points on each side of the square and all $4n + 1$ points are distinct.</p>

## Output

<p>Print two integers&nbsp;— the coordinates of the point that is not on the boundary of the square.</p>





```input1
2
0 0
0 1
0 2
1 0
1 1
1 2
2 0
2 1
2 2
```




```input2
2
0 0
0 1
0 2
0 3
1 0
1 2
2 0
2 1
2 2
```




```output1
1 1
```




```output2
0 3
```



## Note

<p>In both examples, the square has four sides $x=0$, $x=2$, $y=0$, $y=2$.</p>
