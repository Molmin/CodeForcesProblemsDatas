## Description

<div><p>Paladin Manao caught the trail of the ancient Book of Evil in a swampy area. This area contains <span class="tex-span"><i>n</i></span> settlements numbered from 1 to <span class="tex-span"><i>n</i></span>. Moving through the swamp is very difficult, so people tramped exactly <span class="tex-span"><i>n</i> - 1</span> paths. Each of these paths connects some pair of settlements and is bidirectional. Moreover, it is possible to reach any settlement from any other one by traversing one or several paths.</p><p>The <span class="tex-font-style-it">distance</span> between two settlements is the minimum number of paths that have to be crossed to get from one settlement to the other one. Manao knows that the Book of Evil has got a damage range <span class="tex-span"><i>d</i></span>. This means that if the Book of Evil is located in some settlement, its damage (for example, emergence of ghosts and werewolves) affects other settlements at distance <span class="tex-span"><i>d</i></span> or less from the settlement where the Book resides.</p><p>Manao has heard of <span class="tex-span"><i>m</i></span> settlements affected by the Book of Evil. Their numbers are <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>m</i></sub></span>. Note that the Book may be affecting other settlements as well, but this has not been detected yet. Manao wants to determine which settlements may contain the Book. Help him with this difficult task.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 100000;&nbsp;0 ≤ <i>d</i> ≤ <i>n</i> - 1</span>). The second line contains <span class="tex-span"><i>m</i></span> distinct space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). Then <span class="tex-span"><i>n</i> - 1</span> lines follow, each line describes a path made in the area. A path is described by a pair of space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> representing the ends of this path.</p></div><div class="output-specification"><p>Print a single number — the number of settlements that may contain the Book of Evil. It is possible that Manao received some controversial information and there is no settlement that may contain the Book. In such case, print 0.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 100000;&nbsp;0 ≤ <i>d</i> ≤ <i>n</i> - 1</span>). The second line contains <span class="tex-span"><i>m</i></span> distinct space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). Then <span class="tex-span"><i>n</i> - 1</span> lines follow, each line describes a path made in the area. A path is described by a pair of space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> representing the ends of this path.</p>

## Output

<p>Print a single number — the number of settlements that may contain the Book of Evil. It is possible that Manao received some controversial information and there is no settlement that may contain the Book. In such case, print 0.</p>





```input1
6 2 3
1 2
1 5
2 3
3 4
4 5
5 6

```




```output1
3

```



## Note

<p>Sample 1. The damage range of the Book of Evil equals 3 and its effects have been noticed in settlements 1 and 2. Thus, it can be in settlements 3, 4 or 5.</p><center> <img class="tex-graphics" src="file://bjgqkxpI.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
