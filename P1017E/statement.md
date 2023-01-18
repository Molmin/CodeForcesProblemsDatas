## Description

<div><p>After the war, the supersonic rocket became the most common public transportation.</p><p>Each supersonic rocket consists of <span class="tex-font-style-bf">two</span> "<span class="tex-font-style-it">engines</span>". Each engine is a set of "<span class="tex-font-style-it">power sources</span>". The first engine has $n$ power sources, and the second one has $m$ power sources. A power source can be described as a point $(x_i, y_i)$ on a 2-D plane. All points in each engine are different.</p><p>You can manipulate each engine <span class="tex-font-style-bf">separately</span>. There are two operations that you can do with each engine. You can do each operation as many times as you want.</p><ol><li> For every power source as a whole in that engine: $(x_i, y_i)$ becomes $(x_i+a, y_i+b)$, $a$ and $b$ can be any real numbers. In other words, all power sources will be shifted.</li><li> For every power source as a whole in that engine: $(x_i, y_i)$ becomes $(x_i \cos \theta - y_i \sin \theta, x_i \sin \theta + y_i \cos \theta)$, $\theta$ can be any real number. In other words, all power sources will be rotated.</li></ol><p>The engines work as follows: after the two engines are powered, their power sources are being combined (here power sources of different engines may coincide). If two power sources $A(x_a, y_a)$ and $B(x_b, y_b)$ exist, then for all real number $k$ that $0 \lt k \lt 1$, a new power source will be created $C_k(kx_a+(1-k)x_b,ky_a+(1-k)y_b)$. <span class="tex-font-style-bf">Then, this procedure will be repeated again with all new and old power sources</span>. After that, the "<span class="tex-font-style-it">power field</span>" from all power sources will be generated (can be considered as an infinite set of all power sources occurred).</p><p>A supersonic rocket is "<span class="tex-font-style-it">safe</span>" if and only if after you manipulate the engines, destroying any power source and then power the engine, the power field generated won't be changed (comparing to the situation where no power source erased). Two power fields are considered the same if and only if any power source in one field belongs to the other one as well.</p><p>Given a supersonic rocket, check whether it is safe or not.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $m$ ($3 \le n, m \le 10^5$)&nbsp;— the number of power sources in each engine.</p><p>Each of the next $n$ lines contains two integers $x_i$ and $y_i$ ($0\leq x_i, y_i\leq 10^8$)&nbsp;— the coordinates of the $i$-th power source in the first engine.</p><p>Each of the next $m$ lines contains two integers $x_i$ and $y_i$ ($0\leq x_i, y_i\leq 10^8$)&nbsp;— the coordinates of the $i$-th power source in the second engine.</p><p>It is guaranteed that there are no two or more power sources that are located in the same point in each engine.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if the supersonic rocket is safe, otherwise "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in an arbitrary case (upper or lower).</p></div>

## Input

<p>The first line contains two integers $n$, $m$ ($3 \le n, m \le 10^5$)&nbsp;— the number of power sources in each engine.</p><p>Each of the next $n$ lines contains two integers $x_i$ and $y_i$ ($0\leq x_i, y_i\leq 10^8$)&nbsp;— the coordinates of the $i$-th power source in the first engine.</p><p>Each of the next $m$ lines contains two integers $x_i$ and $y_i$ ($0\leq x_i, y_i\leq 10^8$)&nbsp;— the coordinates of the $i$-th power source in the second engine.</p><p>It is guaranteed that there are no two or more power sources that are located in the same point in each engine.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if the supersonic rocket is safe, otherwise "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in an arbitrary case (upper or lower).</p>





```input1
3 4
0 0
0 2
2 0
0 2
2 2
2 0
1 1

```




```input2
3 4
0 0
0 2
2 0
0 2
2 2
2 0
0 0

```




```output1
YES

```




```output2
NO

```



## Note

<p>The first sample:</p><center> <img class="tex-graphics" src="file://WxrRIqh3.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Those near pairs of blue and orange points actually coincide.</span> </center><p>First, manipulate the first engine: use the second operation with $\theta = \pi$ (to rotate all power sources $180$ degrees).</p><p>The power sources in the first engine become $(0, 0)$, $(0, -2)$, and $(-2, 0)$.</p><center> <img class="tex-graphics" src="file://mTxETiI1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Second, manipulate the second engine: use the first operation with $a = b = -2$.</p><p>The power sources in the second engine become $(-2, 0)$, $(0, 0)$, $(0, -2)$, and $(-1, -1)$.</p><center> <img class="tex-graphics" src="file://RoIpnYKT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You can examine that destroying any point, the power field formed by the two engines are always the solid triangle $(0, 0)$, $(-2, 0)$, $(0, -2)$.</p><p>In the second sample, no matter how you manipulate the engines, there always exists a power source in the second engine that power field will shrink if you destroy it. </p>
