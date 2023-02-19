## Description

<div><p>Life has been discovered on Venus! What is more, the life forms appear to be convex polygons. An international consortium is designing a probe to send to Venus to take pictures, but they need to estimate the bandwidth needed to send back pictures.</p><p>When the probe takes a picture of a life form and wishes to send it back to Earth, the bandwidth required is proportional to the area of the bounding box (in other words, the smallest axis-aligned rectangle that contains the life-form). The shape and size of the life forms are known, but the orientation relative to the camera is random. You must thus determine the <span class="tex-font-style-underline">expected</span> (average) area of the bounding box across all orientations.</p></div><div class="input-specification"><p>The input describes the shape of a life form as a convex polygon in two dimensions.</p><p>The first line of input contains an integer $n$ ($3 \le n \le 200\,000$)&nbsp;— the number of vertices. The remaining $n$ lines each contain two integers $x$ and $y$ ($-10^9 \le x, y \le 10^9$)&nbsp;— the coordinates of a vertex. The vertices are given in counterclockwise order, and no three vertices lie on a straight line.</p></div><div class="output-specification"><p>Output a single line containing the expected area of the bounding box of the polygon. Your answer should have an absolute or relative error of at most $10^{-6}$.</p></div>

## Input

<p>The input describes the shape of a life form as a convex polygon in two dimensions.</p><p>The first line of input contains an integer $n$ ($3 \le n \le 200\,000$)&nbsp;— the number of vertices. The remaining $n$ lines each contain two integers $x$ and $y$ ($-10^9 \le x, y \le 10^9$)&nbsp;— the coordinates of a vertex. The vertices are given in counterclockwise order, and no three vertices lie on a straight line.</p>

## Output

<p>Output a single line containing the expected area of the bounding box of the polygon. Your answer should have an absolute or relative error of at most $10^{-6}$.</p>





```input1
4
0 0
10 0
10 10
0 10
```




```input2
5
0 0
10 0
15 8
5 20
-5 7
```




```output1
163.661977237
```




```output2
365.666028588
```



## Note

<p>The pictures show example life forms and various camera orientations. </p><center> <img class="tex-graphics" src="file://3HDBMAcg.png" style="max-width: 100.0%;max-height: 100.0%;"> &nbsp;&nbsp;&nbsp; <img class="tex-graphics" src="file://doNde9s0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
