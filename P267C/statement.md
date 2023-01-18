## Description

<div><p>Berland traffic is very different from traffic in other countries. The capital of Berland consists of <span class="tex-span"><i>n</i></span> junctions and <span class="tex-span"><i>m</i></span> roads. Each road connects a pair of junctions. There can be multiple roads between a pair of junctions. For each road we know its capacity: value <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the maximum number of cars that can drive along a road in any direction per a unit of time. For each road, the cars can drive along it in one of two direction. That it, the cars can't simultaneously move in both directions. A road's traffic is the number of cars that goes along it per a unit of time. For road (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span>) this value is negative, if the traffic moves from <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. A road's traffic can be a non-integer number.</p><p>The capital has two special junctions — the entrance to the city (junction 1) and the exit from the city (junction <span class="tex-span"><i>n</i></span>). For all other junctions it is true that the traffic is not lost there. That is, for all junctions except for 1 and <span class="tex-span"><i>n</i></span> the incoming traffic sum equals the outgoing traffic sum.</p><p>Traffic has an unusual peculiarity in the capital of Berland — for any pair of junctions (<span class="tex-span"><i>x</i>, <i>y</i></span>) the sum of traffics along any path from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> doesn't change depending on the choice of the path. Such sum includes traffic along all roads on the path (possible with the "minus" sign, if the traffic along the road is directed against the direction of the road on the path from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span>).</p><p>Your task is to find the largest traffic that can pass trough the city per one unit of time as well as the corresponding traffic for each road. </p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> — the number of junctions (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>). The second line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 5000</span>) — the number of roads. Next <span class="tex-span"><i>m</i></span> lines contain the roads' descriptions. Each road contains a group of three numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of junctions, connected by the given road, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>) is the largest permissible traffic along this road.</p></div><div class="output-specification"><p>In the first line print the required largest traffic across the city. Then print <span class="tex-span"><i>m</i></span> lines, on each line print the speed, at which the traffic moves along the corresponding road. If the direction doesn't match the order of the junctions, given in the input, then print the traffic with the minus sign. Print the numbers with accuracy of at least five digits after the decimal point.</p><p>If there are many optimal solutions, print any of them.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> — the number of junctions (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>). The second line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 5000</span>) — the number of roads. Next <span class="tex-span"><i>m</i></span> lines contain the roads' descriptions. Each road contains a group of three numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of junctions, connected by the given road, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>) is the largest permissible traffic along this road.</p>

## Output

<p>In the first line print the required largest traffic across the city. Then print <span class="tex-span"><i>m</i></span> lines, on each line print the speed, at which the traffic moves along the corresponding road. If the direction doesn't match the order of the junctions, given in the input, then print the traffic with the minus sign. Print the numbers with accuracy of at least five digits after the decimal point.</p><p>If there are many optimal solutions, print any of them.</p>





```input1
2
3
1 2 2
1 2 4
2 1 1000

```




```input2
7
11
1 2 7
1 2 7
1 3 7
1 4 7
2 3 7
2 5 7
3 6 7
4 7 7
5 4 7
5 6 7
6 7 7

```




```output1
6.00000
2.00000
2.00000
-2.00000

```




```output2
13.00000
2.00000
2.00000
3.00000
6.00000
1.00000
3.00000
4.00000
7.00000
1.00000
2.00000
6.00000

```


