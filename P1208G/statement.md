## Description

<div><p>You are given two integers $n$ and $k$.</p><p>You need to construct $k$ regular polygons having same <a href="https://en.wikipedia.org/wiki/Circumscribed_circle">circumcircle</a>, with <span class="tex-font-style-bf">distinct</span> number of sides $l$ between $3$ and $n$. </p><center> <img class="tex-graphics" src="file://nFN7WNcu.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Illustration for the first example.</span> </center><p>You can rotate them to minimize the total number of distinct points on the circle. Find the minimum number of such points.</p></div><div class="input-specification"><p>The only line of input contains two integers $n$ and $k$ ($3 \le n \le 10^{6}$, $1 \le k \le n-2$), the maximum number of sides of a polygon and the number of polygons to construct, respectively.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of points required for $k$ polygons.</p></div>

## Input

<p>The only line of input contains two integers $n$ and $k$ ($3 \le n \le 10^{6}$, $1 \le k \le n-2$), the maximum number of sides of a polygon and the number of polygons to construct, respectively.</p>

## Output

<p>Print a single integer — the minimum number of points required for $k$ polygons.</p>





```input1
6 2
```




```input2
200 50
```




```output1
6
```




```output2
708
```



## Note

<p>In the first example, we have $n = 6$ and $k = 2$. So, we have $4$ polygons with number of sides $3$, $4$, $5$ and $6$ to choose from and if we choose the triangle and the hexagon, then we can arrange them as shown in the picture in the statement.</p><p>Hence, the minimum number of points required on the circle is $6$, which is also the minimum overall possible sets.</p>
