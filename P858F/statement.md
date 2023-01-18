## Description

<div><p>All Berland residents are waiting for an unprecedented tour of wizard in his Blue Helicopter over the cities of Berland!</p><p>It is well-known that there are <span class="tex-span"><i>n</i></span> cities in Berland, some pairs of which are connected by bidirectional roads. Each pair of cities is connected by no more than one road. It is not guaranteed that the road network is <span class="tex-font-style-it">connected</span>, i.e. it is possible that you can't reach some city from some other.</p><p>The tour will contain several episodes. In each of the episodes:</p><ul> <li> the wizard will disembark at some city <span class="tex-span"><i>x</i></span> from the Helicopter; </li><li> he will give a performance and show a movie for free at the city <span class="tex-span"><i>x</i></span>; </li><li> he will drive to some neighboring city <span class="tex-span"><i>y</i></span> using a road; </li><li> he will give a performance and show a movie for free at the city <span class="tex-span"><i>y</i></span>; </li><li> he will drive to some neighboring to <span class="tex-span"><i>y</i></span> city <span class="tex-span"><i>z</i></span>; </li><li> he will give a performance and show a movie for free at the city <span class="tex-span"><i>z</i></span>; </li><li> he will embark the Helicopter and fly away from the city <span class="tex-span"><i>z</i></span>. </li></ul><p>It is known that the wizard doesn't like to use roads, so he agrees to use each road at most once (regardless of direction). In other words, for road between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> he only can drive once from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>, or drive once from <span class="tex-span"><i>b</i></span> to <span class="tex-span"><i>a</i></span>, or do not use this road at all.</p><p>The wizards wants to plan as many episodes as possible without violation the above rules. Help the wizard!</p><p>Please note that the wizard can visit the same city multiple times, the restriction is on roads only.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of cities and the number of roads in Berland, respectively.</p><p>The roads description follow, one in each line. Each description is a pair of two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the ids of the cities connected by the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that there are no two roads connecting the same pair of cities. Every road is bidirectional. The cities are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>It is possible that the road network in Berland is not connected.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>w</i></span> — the maximum possible number of episodes. The next <span class="tex-span"><i>w</i></span> lines should contain the episodes in format <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>z</i></span> — the three integers denoting the ids of the cities in the order of the wizard's visits.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of cities and the number of roads in Berland, respectively.</p><p>The roads description follow, one in each line. Each description is a pair of two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the ids of the cities connected by the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that there are no two roads connecting the same pair of cities. Every road is bidirectional. The cities are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>It is possible that the road network in Berland is not connected.</p>

## Output

<p>In the first line print <span class="tex-span"><i>w</i></span> — the maximum possible number of episodes. The next <span class="tex-span"><i>w</i></span> lines should contain the episodes in format <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>z</i></span> — the three integers denoting the ids of the cities in the order of the wizard's visits.</p>





```input1
4 5
1 2
3 2
2 4
3 4
4 1

```




```input2
5 8
5 3
1 2
4 5
5 1
2 5
4 3
1 4
3 2

```




```output1
2
1 4 2
4 3 2

```




```output2
4
1 4 5
2 3 4
1 5 3
5 2 1

```


