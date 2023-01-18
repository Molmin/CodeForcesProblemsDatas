## Description

<div><p>As a result of Pinky and Brain's mysterious experiments in the Large Hadron Collider some portals or black holes opened to the parallel dimension. And the World Evil has crept to the veil between their world and ours. Brain quickly evaluated the situation and he understood that the more evil tentacles creep out and become free, the higher is the possibility that Brain will rule the world.</p><p>The collider's constriction is a rectangular grid rolled into a cylinder and consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns such as is shown in the picture below:</p><center> <img class="tex-graphics" src="file://nn6tA8Cu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In this example <span class="tex-span"><i>n</i> = 4</span>, <span class="tex-span"><i>m</i> = 5</span>. Dotted lines are corridores that close each column to a ring, i. e. connect the <span class="tex-span"><i>n</i></span>-th and the <span class="tex-span">1</span>-th rows of the grid.</p><p>In the leftmost column of the grid the portals are situated and the tentacles of the World Evil are ready to creep out from there. In the rightmost column the exit doors are located. The tentacles can only get out through those doors. The segments joining the nodes of the grid are corridors.</p><p>Brain would be glad to let all the tentacles out but he faces a problem: the infinite number of tentacles can creep out of the portals, every tentacle possesses infinite length and some width and the volume of the corridors are, unfortunately, quite limited. Brain could approximately evaluate the maximal number of tentacles that will be able to crawl through every corridor.</p><p>Now help the mice to determine the maximal number of tentacles of the World Evil that will crawl out of the Large Hadron Collider.</p></div><div class="input-specification"><p>The first line of the input file contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5</span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). They are the sizes of the Large Hadron Collider grid. The next <span class="tex-span"><i>m</i> - 1</span> lines contain <span class="tex-span"><i>n</i></span> numbers each. They are the horizontal corridors' capacities. The next <span class="tex-span"><i>m</i></span> lines contain <span class="tex-span"><i>n</i></span> numbers each. They are the vertical corridors' capacities. Corridors are described from left to right and from top to bottom. Every <span class="tex-span"><i>n</i></span>-th vertical corridor connects nodes of the <span class="tex-span"><i>n</i></span>-th and <span class="tex-span">1</span>-th rows. A corridor's capacity is a non-negative integer that does not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>Print a single number, the number of the World Evil tentacles Pinky and Brain will command.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line of the input file contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5</span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). They are the sizes of the Large Hadron Collider grid. The next <span class="tex-span"><i>m</i> - 1</span> lines contain <span class="tex-span"><i>n</i></span> numbers each. They are the horizontal corridors' capacities. The next <span class="tex-span"><i>m</i></span> lines contain <span class="tex-span"><i>n</i></span> numbers each. They are the vertical corridors' capacities. Corridors are described from left to right and from top to bottom. Every <span class="tex-span"><i>n</i></span>-th vertical corridor connects nodes of the <span class="tex-span"><i>n</i></span>-th and <span class="tex-span">1</span>-th rows. A corridor's capacity is a non-negative integer that does not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>Print a single number, the number of the World Evil tentacles Pinky and Brain will command.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
3 4
4 4 4
1 1 5
5 5 3
4 1 2
1 3 1
3 5 4
1 4 3

```




```input2
2 2
9 2
2 3
6 1

```




```output1
7

```




```output2
11

```


