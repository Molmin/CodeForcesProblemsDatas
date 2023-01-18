## Description

<div><p>A country called Berland consists of <span class="tex-span"><i>n</i></span> cities, numbered with integer numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some of them are connected by bidirectional roads. Each road has some length. There is a path from each city to any other one by these roads. According to some Super Duper Documents, Berland is protected by the Super Duper Missiles. The exact position of the Super Duper Secret Missile Silos is kept secret but Bob managed to get hold of the information. That information says that all silos are located exactly at a distance <span class="tex-span"><i>l</i></span> from the capital. The capital is located in the city with number <span class="tex-span"><i>s</i></span>.</p><p>The documents give the formal definition: the Super Duper Secret Missile Silo is located at some place (which is either city or a point on a road) if and only if the shortest distance from this place to the capital along the roads of the country equals exactly <span class="tex-span"><i>l</i></span>.</p><p>Bob wants to know how many missile silos are located in Berland to sell the information then to enemy spies. Help Bob.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <img align="middle" class="tex-formula" src="file://oX5OFOfq.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>) — the number of cities, the number of roads in the country and the number of the capital, correspondingly. Capital is the city no. <span class="tex-span"><i>s</i></span>. </p><p>Then <span class="tex-span"><i>m</i></span> lines contain the descriptions of roads. Each of them is described by three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> are numbers of the cities connected by this road and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is its length. The last input line contains integer <span class="tex-span"><i>l</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>) — the distance from the capital to the missile silos. It is guaranteed that: </p><ul> <li> between any two cities no more than one road exists; </li><li> each road connects two different cities; </li><li> from each city there is at least one way to any other city by the roads. </li></ul></div><div class="output-specification"><p>Print the single number — the number of Super Duper Secret Missile Silos that are located in Berland.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <img align="middle" class="tex-formula" src="file://oX5OFOfq.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>) — the number of cities, the number of roads in the country and the number of the capital, correspondingly. Capital is the city no. <span class="tex-span"><i>s</i></span>. </p><p>Then <span class="tex-span"><i>m</i></span> lines contain the descriptions of roads. Each of them is described by three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> are numbers of the cities connected by this road and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is its length. The last input line contains integer <span class="tex-span"><i>l</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>) — the distance from the capital to the missile silos. It is guaranteed that: </p><ul> <li> between any two cities no more than one road exists; </li><li> each road connects two different cities; </li><li> from each city there is at least one way to any other city by the roads. </li></ul>

## Output

<p>Print the single number — the number of Super Duper Secret Missile Silos that are located in Berland.</p>





```input1
4 6 1
1 2 1
1 3 3
2 3 1
2 4 1
3 4 1
1 4 2
2

```




```input2
5 6 3
3 1 1
3 2 1
3 4 1
3 5 1
1 2 6
4 5 8
4

```




```output1
3

```




```output2
3

```



## Note

<p>In the first sample the silos are located in cities <span class="tex-span">3</span> and <span class="tex-span">4</span> and on road <span class="tex-span">(1, 3)</span> at a distance <span class="tex-span">2</span> from city <span class="tex-span">1</span> (correspondingly, at a distance <span class="tex-span">1</span> from city <span class="tex-span">3</span>).</p><p>In the second sample one missile silo is located right in the middle of the road <span class="tex-span">(1, 2)</span>. Two more silos are on the road <span class="tex-span">(4, 5)</span> at a distance <span class="tex-span">3</span> from city <span class="tex-span">4</span> in the direction to city <span class="tex-span">5</span> and at a distance <span class="tex-span">3</span> from city <span class="tex-span">5</span> to city <span class="tex-span">4</span>.</p>
