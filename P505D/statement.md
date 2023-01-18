## Description

<div><p>Shuseki Kingdom is the world's leading nation for innovation and technology. There are <span class="tex-span"><i>n</i></span> cities in the kingdom, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>Thanks to Mr. Kitayuta's research, it has finally become possible to construct teleportation pipes between two cities. A teleportation pipe will connect two cities unidirectionally, that is, a teleportation pipe from city <span class="tex-span"><i>x</i></span> to city <span class="tex-span"><i>y</i></span> cannot be used to travel from city <span class="tex-span"><i>y</i></span> to city <span class="tex-span"><i>x</i></span>. The transportation within each city is extremely developed, therefore if a pipe from city <span class="tex-span"><i>x</i></span> to city <span class="tex-span"><i>y</i></span> and a pipe from city <span class="tex-span"><i>y</i></span> to city <span class="tex-span"><i>z</i></span> are both constructed, people will be able to travel from city <span class="tex-span"><i>x</i></span> to city <span class="tex-span"><i>z</i></span> instantly.</p><p>Mr. Kitayuta is also involved in national politics. He considers that the transportation between the <span class="tex-span"><i>m</i></span> pairs of city <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) is important. He is planning to construct teleportation pipes so that for each important pair <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, it will be possible to travel from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> by using one or more teleportation pipes (but not necessarily from city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>). Find the minimum number of teleportation pipes that need to be constructed. So far, no teleportation pipe has been constructed, and there is no other effective transportation between cities.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of the cities in Shuseki Kingdom and the number of the important pairs, respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines describe the important pairs. The <span class="tex-span"><i>i</i></span>-th of them (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), denoting that it must be possible to travel from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> by using one or more teleportation pipes (but not necessarily from city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>). It is guaranteed that all pairs <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> are distinct.</p></div><div class="output-specification"><p>Print the minimum required number of teleportation pipes to fulfill Mr. Kitayuta's purpose.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of the cities in Shuseki Kingdom and the number of the important pairs, respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines describe the important pairs. The <span class="tex-span"><i>i</i></span>-th of them (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), denoting that it must be possible to travel from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> by using one or more teleportation pipes (but not necessarily from city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>). It is guaranteed that all pairs <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> are distinct.</p>

## Output

<p>Print the minimum required number of teleportation pipes to fulfill Mr. Kitayuta's purpose.</p>





```input1
4 5
1 2
1 3
1 4
2 3
2 4

```




```input2
4 6
1 2
1 4
2 3
2 4
3 2
3 4

```




```output1
3

```




```output2
4

```



## Note

<p>For the first sample, one of the optimal ways to construct pipes is shown in the image below: </p><center> <img class="tex-graphics" src="file://oh0ZYHFv.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the second sample, one of the optimal ways is shown below: </p><center> <img class="tex-graphics" src="file://3R3MLm4r.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
