## Description

<div><p>Sehr Sus is an infinite hexagonal grid as pictured below, controlled by MennaFadali, ZerooCool and Hosssam.</p><p>They love equilateral triangles and want to create $n$ equilateral triangles on the grid by adding some straight lines. The triangles must all be empty from the inside (in other words, no straight line or hexagon edge should pass through any of the triangles).</p><p>You are allowed to add straight lines parallel to the edges of the hexagons. Given $n$, what is the minimum number of lines you need to add to create at least $n$ equilateral triangles as described?</p><center> <img class="tex-graphics" src="file://ZNJtI7Wg.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Adding two red lines results in two new yellow equilateral triangles.</span> </center></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case contains a single integer $n$ ($1 \le n \le 10^{9}$) — the required number of equilateral triangles.</p></div><div class="output-specification"><p>For each test case, print the minimum number of lines needed to have $n$ or more equilateral triangles.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case contains a single integer $n$ ($1 \le n \le 10^{9}$) — the required number of equilateral triangles.</p>

## Output

<p>For each test case, print the minimum number of lines needed to have $n$ or more equilateral triangles.</p>





```input1
4
1
2
3
4567
```




```output1
2
2
3
83
```



## Note

<p>In the first and second test cases only 2 lines are needed. After adding the first line, no equilateral triangles will be created no matter where it is added. But after adding the second line, two more triangles will be created at once. </p><center> <img class="tex-graphics" src="file://KlSNV912.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third test case, the minimum needed is 3 lines as shown below.</p><center> <img class="tex-graphics" src="file://r2cNMPfZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
