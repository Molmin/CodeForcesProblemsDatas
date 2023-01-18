## Description

<div><p>According to the last order issued by the president of Berland every city of the country must have its own Ministry Defense building (their own Pentagon). A megapolis Berbourg was not an exception. This city has <span class="tex-span"><i>n</i></span> junctions, some pairs of which are connected by two-way roads. Overall there are <span class="tex-span"><i>m</i></span> roads in the city, no more than one between each pair of junctions.</p><p>At the moment choosing a location place for Pentagon in Berbourg is being discussed. It has been decided that Pentagon should cover the territory of five different junctions which are joined into a cycle by roads. In the order to build Pentagon a special wall will be built along the roads (with high-tension razor, high-voltage wire and other attributes). Thus, the number of possible ways of building Pentagon in the city is equal to the number of different cycles at lengths of 5, composed of junctions and roads.</p><p>Your task is to prints the number of ways of building Pentagon in Berbourg. Only well-optimized solutions will be accepted. Please, test your code on the maximal testcase.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 700;0 ≤ <i>m</i> ≤ <i>n</i>·(<i>n</i> - 1) / 2</span>), where <span class="tex-span"><i>n</i></span> represents the number of junctions and <span class="tex-span"><i>m</i></span> is the number of roads in the city. Then follow <span class="tex-span"><i>m</i></span> lines containing the road descriptions, one in each line. Every road is set by a number of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> represent the numbers of junctions, connected by the road. The junctions are numbered from 1 to <span class="tex-span"><i>n</i></span>. It is not guaranteed that from any junction one can get to any other one moving along the roads.</p></div><div class="output-specification"><p>Print the single number which represents the required number of ways. Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 700;0 ≤ <i>m</i> ≤ <i>n</i>·(<i>n</i> - 1) / 2</span>), where <span class="tex-span"><i>n</i></span> represents the number of junctions and <span class="tex-span"><i>m</i></span> is the number of roads in the city. Then follow <span class="tex-span"><i>m</i></span> lines containing the road descriptions, one in each line. Every road is set by a number of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> represent the numbers of junctions, connected by the road. The junctions are numbered from 1 to <span class="tex-span"><i>n</i></span>. It is not guaranteed that from any junction one can get to any other one moving along the roads.</p>

## Output

<p>Print the single number which represents the required number of ways. Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
5 5
1 2
2 3
3 4
4 5
5 1

```




```input2
5 10
1 2
1 3
1 4
1 5
2 3
2 4
2 5
3 4
3 5
4 5

```




```output1
1

```




```output2
12

```


