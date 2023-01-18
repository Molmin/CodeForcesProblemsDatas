## Description

<div><p><span class="tex-font-style-it">This problem is same as the next one, but has smaller constraints.</span></p><p>It was a Sunday morning when the three friends Selena, Shiro and Katie decided to have a trip to the nearby power station <span class="tex-font-style-it">(do not try this at home)</span>. After arriving at the power station, the cats got impressed with a large power transmission system consisting of many chimneys, electric poles, and wires. Since they are cats, they found those things gigantic.</p><p>At the entrance of the station, there is a map describing the complicated wiring system. Selena is the best at math among three friends. He decided to draw the map on the Cartesian plane. Each pole is now a point at some coordinates $(x_i, y_i)$. Since every pole is different, all of the points representing these poles are distinct. Also, every two poles are connected with each other by wires. A wire is a straight line on the plane <span class="tex-font-style-bf">infinite in both directions</span>. If there are more than two poles lying on the same line, they are connected by a single common wire.</p><p>Selena thinks, that whenever two different electric wires intersect, they may interfere with each other and cause damage. So he wonders, how many pairs are intersecting? Could you help him with this problem?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 50$)&nbsp;— the number of electric poles.</p><p>Each of the following $n$ lines contains two integers $x_i$, $y_i$ ($-10^4 \le x_i, y_i \le 10^4$)&nbsp;— the coordinates of the poles.</p><p>It is guaranteed that all of these $n$ points are distinct.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of pairs of wires that are intersecting.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 50$)&nbsp;— the number of electric poles.</p><p>Each of the following $n$ lines contains two integers $x_i$, $y_i$ ($-10^4 \le x_i, y_i \le 10^4$)&nbsp;— the coordinates of the poles.</p><p>It is guaranteed that all of these $n$ points are distinct.</p>

## Output

<p>Print a single integer&nbsp;— the number of pairs of wires that are intersecting.</p>





```input1
4
0 0
1 1
0 3
1 2
```




```input2
4
0 0
0 2
0 4
2 0
```




```input3
3
-1 -1
1 0
3 1
```




```output1
14
```




```output2
6
```




```output3
0
```



## Note

<p>In the first example:</p><center> <img class="tex-graphics" src="file://73iJRN2K.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example:</p><center> <img class="tex-graphics" src="file://40DwUdOP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that the three poles $(0, 0)$, $(0, 2)$ and $(0, 4)$ are connected by a single wire.</p><p>In the third example:</p><center> <img class="tex-graphics" src="file://DGLhFwIm.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
