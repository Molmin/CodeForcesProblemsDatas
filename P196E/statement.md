## Description

<div><p>Pavel plays a famous computer game. A player is responsible for a whole country and he can travel there freely, complete quests and earn experience.</p><p>This country has <span class="tex-span"><i>n</i></span> cities connected by <span class="tex-span"><i>m</i></span> bidirectional roads of different lengths so that it is possible to get from any city to any other one. There are portals in <span class="tex-span"><i>k</i></span> of these cities. At the beginning of the game all portals are closed. When a player visits a portal city, the portal opens. Strange as it is, one can teleport from an open portal to an open one. The teleportation takes no time and that enables the player to travel quickly between rather remote regions of the country.</p><p>At the beginning of the game Pavel is in city number <span class="tex-span">1</span>. He wants to open all portals as quickly as possible. How much time will he need for that?</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) that show how many cities and roads are in the game.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of a road as three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the numbers of the cities connected by the <span class="tex-span"><i>i</i></span>-th road and the time needed to go from one city to the other one by this road. Any two cities are connected by no more than one road. It is guaranteed that we can get from any city to any other one, moving along the roads of the country.</p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of portals.</p><p>The next line contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i></sub></span> — numbers of the cities with installed portals. Each city has no more than one portal.</p></div><div class="output-specification"><p>Print a single number — the minimum time a player needs to open all portals.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) that show how many cities and roads are in the game.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of a road as three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the numbers of the cities connected by the <span class="tex-span"><i>i</i></span>-th road and the time needed to go from one city to the other one by this road. Any two cities are connected by no more than one road. It is guaranteed that we can get from any city to any other one, moving along the roads of the country.</p><p>The next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of portals.</p><p>The next line contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i></sub></span> — numbers of the cities with installed portals. Each city has no more than one portal.</p>

## Output

<p>Print a single number — the minimum time a player needs to open all portals.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3 3
1 2 1
1 3 1
2 3 1
3
1 2 3

```




```input2
4 3
1 2 1
2 3 5
2 4 10
3
2 3 4

```




```input3
4 3
1 2 1000000000
2 3 1000000000
3 4 1000000000
4
1 2 3 4

```




```output1
2

```




```output2
16

```




```output3
3000000000

```



## Note

<p>In the second sample the player has to come to city <span class="tex-span">2</span>, open a portal there, then go to city <span class="tex-span">3</span>, open a portal there, teleport back to city <span class="tex-span">2</span> and finally finish the journey in city <span class="tex-span">4</span>.</p>
