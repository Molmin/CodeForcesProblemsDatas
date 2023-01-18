## Description

<div><p>It has been noted that if some ants are put in the junctions of the graphene integer lattice then they will act in the following fashion: every minute at each junction (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>) containing at least four ants a group of four ants will be formed, and these four ants will scatter to the neighbouring junctions (<span class="tex-span"><i>x</i> + 1</span>, <span class="tex-span"><i>y</i></span>), (<span class="tex-span"><i>x</i> - 1</span>, <span class="tex-span"><i>y</i></span>), (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i> + 1</span>), (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i> - 1</span>) — one ant in each direction. No other ant movements will happen. Ants never interfere with each other.</p><p>Scientists have put a colony of <span class="tex-span"><i>n</i></span> ants into the junction (0, 0) and now they wish to know how many ants will there be at some given junctions, when the movement of the ants stops.</p></div><div class="input-specification"><p>First input line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 30000</span>) and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 50000</span>), where <span class="tex-span"><i>n</i></span> is the number of ants in the colony and <span class="tex-span"><i>t</i></span> is the number of queries. Each of the next <span class="tex-span"><i>t</i></span> lines contains coordinates of a query junction: integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Queries may coincide.</p><p>It is guaranteed that there will be a certain moment of time when no possible movements can happen (in other words, the process will eventually end).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> integers, one per line — the number of ants at the corresponding junctions when the movement of the ants stops.</p></div>

## Input

<p>First input line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 30000</span>) and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 50000</span>), where <span class="tex-span"><i>n</i></span> is the number of ants in the colony and <span class="tex-span"><i>t</i></span> is the number of queries. Each of the next <span class="tex-span"><i>t</i></span> lines contains coordinates of a query junction: integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Queries may coincide.</p><p>It is guaranteed that there will be a certain moment of time when no possible movements can happen (in other words, the process will eventually end).</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> integers, one per line — the number of ants at the corresponding junctions when the movement of the ants stops.</p>





```input1
1 3
0 1
0 0
0 -1

```




```input2
6 5
0 -2
0 -1
0 0
0 1
0 2

```




```output1
0
1
0

```




```output2
0
1
2
1
0

```



## Note

<p>In the first sample the colony consists of the one ant, so nothing happens at all.</p><p>In the second sample the colony consists of 6 ants. At the first minute 4 ants scatter from (0, 0) to the neighbouring junctions. After that the process stops.</p>
