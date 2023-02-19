## Description

<div><p>Mahmoud and Ehab live in a country with <span class="tex-span"><i>n</i></span> cities numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and connected by <span class="tex-span"><i>n</i> - 1</span> undirected roads. It's guaranteed that you can reach any city from any other using these roads. Each city has a number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> attached to it.</p><p>We define the distance from city <span class="tex-span"><i>x</i></span> to city <span class="tex-span"><i>y</i></span> as the <span class="tex-font-style-tt">xor</span> of numbers attached to the cities on the path from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> <span class="tex-font-style-bf">(including both <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>)</span>. In other words if values attached to the cities on the path from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> form an array <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>l</i></span> then the distance between them is <img align="middle" class="tex-formula" src="file://FWN6j2I9.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://wqxyGtUd.png" style="max-width: 100.0%;max-height: 100.0%;"> is bitwise <span class="tex-font-style-tt">xor</span> operation.</p><p>Mahmoud and Ehab want to choose two cities and make a journey from one to another. The index of the start city is always less than or equal to the index of the finish city (they may start and finish in the same city and in this case the distance equals the number attached to that city). They can't determine the two cities so they try every city as a start and every city with greater index as a finish. They want to know the total distance between all pairs of cities.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities in Mahmoud and Ehab's country.</p><p>Then the second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) which represent the numbers attached to the cities. Integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is attached to the city <span class="tex-span"><i>i</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i>  -  1</span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1  ≤  <i>u</i>,  <i>v</i>  ≤  <i>n</i></span>, <span class="tex-span"><i>u</i>  ≠  <i>v</i></span>), denoting that there is an undirected road between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It's guaranteed that you can reach any city from any other using these roads.</p></div><div class="output-specification"><p>Output one number denoting the total distance between all pairs of cities.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities in Mahmoud and Ehab's country.</p><p>Then the second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) which represent the numbers attached to the cities. Integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is attached to the city <span class="tex-span"><i>i</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i>  -  1</span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1  ≤  <i>u</i>,  <i>v</i>  ≤  <i>n</i></span>, <span class="tex-span"><i>u</i>  ≠  <i>v</i></span>), denoting that there is an undirected road between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It's guaranteed that you can reach any city from any other using these roads.</p>

## Output

<p>Output one number denoting the total distance between all pairs of cities.</p>





```input1
3
1 2 3
1 2
2 3

```




```input2
5
1 2 3 4 5
1 2
2 3
3 4
3 5

```




```input3
5
10 9 8 7 6
1 2
2 3
3 4
3 5

```




```output1
10

```




```output2
52

```




```output3
131

```



## Note

<p>A bitwise <span class="tex-font-style-tt">xor</span> takes two bit integers of equal length and performs the logical <span class="tex-font-style-tt">xor</span> operation on each pair of corresponding bits. The result in each position is <span class="tex-span">1</span> if only the first bit is <span class="tex-span">1</span> or only the second bit is <span class="tex-span">1</span>, but will be <span class="tex-span">0</span> if both are <span class="tex-span">0</span> or both are <span class="tex-span">1</span>. You can read more about bitwise <span class="tex-font-style-tt">xor</span> operation here: <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">https://en.wikipedia.org/wiki/Bitwise_operation#XOR</a>.</p><p>In the first sample the available paths are:</p><ul> <li> city <span class="tex-span">1</span> to itself with a distance of <span class="tex-span">1</span>, </li><li> city <span class="tex-span">2</span> to itself with a distance of <span class="tex-span">2</span>, </li><li> city <span class="tex-span">3</span> to itself with a distance of <span class="tex-span">3</span>, </li><li> city <span class="tex-span">1</span> to city <span class="tex-span">2</span> with a distance of <img align="middle" class="tex-formula" src="file://ccgNvbGU.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> city <span class="tex-span">1</span> to city <span class="tex-span">3</span> with a distance of <img align="middle" class="tex-formula" src="file://4mVzgPDD.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> city <span class="tex-span">2</span> to city <span class="tex-span">3</span> with a distance of <img align="middle" class="tex-formula" src="file://X4vN5DzO.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul> The total distance between all pairs of cities equals <span class="tex-span">1 + 2 + 3 + 3 + 0 + 1 = 10</span>.
