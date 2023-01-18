## Description

<div><p>A new bus route is opened in the city <img align="middle" class="tex-formula" src="file://M5j3bBtF.png" style="max-width: 100.0%;max-height: 100.0%;">. The route is a closed polygon line in the place, with all segments parallel to one of the axes. <span class="tex-span"><i>m</i></span> buses will operate on the route. All buses move in a loop along the route in the same direction with equal constant velocities (stopping times are negligible in this problem).</p><p>Buses start their movement in the first vertex of the route with equal interval. Suppose that <span class="tex-span"><i>T</i></span> is the total time for a single bus to travel the whole loop of the route. Then, the bus 1 starts moving at time 0, the bus 2 starts at time <span class="tex-span"><i>T</i> / <i>m</i></span>, the bus 3 starts at time <span class="tex-span">2<i>T</i> / <i>m</i></span>, and so on; finally, the bus <span class="tex-span"><i>m</i></span> starts moving at time <span class="tex-span">(<i>m</i> - 1)<i>T</i> / <i>m</i></span>. Thus, all intervals between pairs of consecutive buses (including the interval between the last and the first bus) are equal.</p><p>Buses can communicate with each other via wireless transmitters of equal power. If the transmitters have power <span class="tex-span"><i>D</i></span>, then only buses within distance <span class="tex-span"><i>D</i></span> of each other can communicate.</p><p>The buses are also equipped with a distributed system of schedule tracking. For all buses to stick to the schedule, the system has to synchronize the necessary data between all buses from time to time. At the moment of synchronization, the bus 1 communicates with the bus 2, the bus 2&nbsp;— with bus 3, and so on; also, the bus <span class="tex-span"><i>m</i></span> communicates with the bus 1.</p><p>As a research employee, you are tasked with finding the smallest value of <span class="tex-span"><i>D</i></span> such that it is possible to find a time moment to perform synchronization once all buses have started moving. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices of the polygonal line, and the number of buses respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the vertices of the route in the traversing order. Each of these lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— coordinates of respective vertex.</p><p>It is guaranteed that each leg of the route (including the leg between the last and the first vertex) is paralles to one of the coordinate axes. Moreover, no two subsequent vertices of the route coincide. The route is allowed to have self-intersections, and travel along the same segment multiple times.</p></div><div class="output-specification"><p>Print one real number&nbsp;— the answer to the problem. Your answer will be accepted if the relative or the absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices of the polygonal line, and the number of buses respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the vertices of the route in the traversing order. Each of these lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— coordinates of respective vertex.</p><p>It is guaranteed that each leg of the route (including the leg between the last and the first vertex) is paralles to one of the coordinate axes. Moreover, no two subsequent vertices of the route coincide. The route is allowed to have self-intersections, and travel along the same segment multiple times.</p>

## Output

<p>Print one real number&nbsp;— the answer to the problem. Your answer will be accepted if the relative or the absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
4 2
0 0
0 1
1 1
1 0

```




```input2
2 2
0 0
1 0

```




```output1
1.000000000

```




```output2
0.000000000
```



## Note

<p>Suppose that each bus travel 1 distance unit per second.</p><p>In the first sample case, in 0.5 seconds buses will be at distance 1, hence we can choose <span class="tex-span"><i>D</i> = 1</span>.</p><p>In the second sample case, in 0.5 seconds both buses will be at <span class="tex-span">(0.5, 0)</span>, hence we can choose <span class="tex-span"><i>D</i> = 0</span>.</p>
