## Description

<div><p>Berland is very concerned with privacy, so almost all plans and blueprints are secret. However, a spy of the neighboring state managed to steal the Bertown subway scheme.</p><p>The Bertown Subway has <span class="tex-span"><i>n</i></span> stations, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and <span class="tex-span"><i>m</i></span> bidirectional tunnels connecting them. All Bertown Subway consists of lines. To be more precise, there are two types of lines: circular and radial.</p><p>A <span class="tex-font-style-it">radial line</span> is a sequence of stations <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, ..., <i>v</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(<i>k</i> &gt; 1)</span>, where stations <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> <span class="tex-span">(<i>i</i> &lt; <i>k</i>)</span> are connected by a tunnel and no station occurs in the line more than once (<span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub></span> for <span class="tex-span"><i>i</i> ≠ <i>j</i></span>).</p><p>A <span class="tex-font-style-it">loop line</span> is a series of stations, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, ..., <i>v</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(<i>k</i> &gt; 2)</span>, where stations <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> и <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> are connected by a tunnel. In addition, stations <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span> are also connected by a tunnel. No station is occurs in the loop line more than once.</p><p>Note that a single station can be passed by any number of lines.</p><p>According to Berland standards, there can't be more than one tunnel between two stations and each tunnel belongs to exactly one line. Naturally, each line has at least one tunnel. Between any two stations there is the way along the subway tunnels. In addition, in terms of graph theory, a subway is a vertex cactus: if we consider the subway as a graph in which the stations are the vertexes and the edges are tunnels, then each vertex lies on no more than one simple cycle.</p><p>Unfortunately, scheme, stolen by the spy, had only the stations and the tunnels. It was impossible to determine to which line every tunnel corresponds. But to sabotage successfully, the spy needs to know what minimum and maximum number of lines may be in the Bertown subway.</p><p>Help him!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of stations and the number of tunnels, correspondingly.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contain two integers — the numbers of stations connected by the corresponding tunnel. The stations are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>It is guaranteed that the graph that corresponds to the subway has no multiple edges or loops, it is connected and it is a vertex cactus.</p></div><div class="output-specification"><p>Print two numbers — the minimum and maximum number of lines correspondingly.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of stations and the number of tunnels, correspondingly.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contain two integers — the numbers of stations connected by the corresponding tunnel. The stations are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>It is guaranteed that the graph that corresponds to the subway has no multiple edges or loops, it is connected and it is a vertex cactus.</p>

## Output

<p>Print two numbers — the minimum and maximum number of lines correspondingly.</p>





```input1
3 3
1 2
2 3
3 1

```




```input2
8 8
1 2
2 3
3 4
4 5
6 4
4 7
7 2
2 8

```




```input3
6 6
1 2
2 3
2 5
5 6
3 4
3 5

```




```output1
1 3

```




```output2
2 8

```




```output3
3 6

```



## Note

<p>The subway scheme with minimum possible number of lines for the second sample is: </p><center> <img class="tex-graphics" src="file://IIiQKSpA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
