## Description

<div><p>Goa'uld Apophis captured Jack O'Neill's team again! Jack himself was able to escape, but by that time Apophis's ship had already jumped to hyperspace. But Jack knows on what planet will Apophis land. In order to save his friends, Jack must repeatedly go through stargates to get to this planet.</p><p>Overall the galaxy has <span class="tex-span"><i>n</i></span> planets, indexed with numbers from 1 to <span class="tex-span"><i>n</i></span>. Jack is on the planet with index 1, and Apophis will land on the planet with index <span class="tex-span"><i>n</i></span>. Jack can move between some pairs of planets through stargates (he can move in both directions); the transfer takes a positive, and, perhaps, for different pairs of planets unequal number of seconds. Jack begins his journey at time 0.</p><p>It can be that other travellers are arriving to the planet where Jack is currently located. In this case, Jack has to wait for exactly 1 second before he can use the stargate. That is, if at time <span class="tex-span"><i>t</i></span> another traveller arrives to the planet, Jack can only pass through the stargate at time <span class="tex-span"><i>t</i> + 1</span>, unless there are more travellers arriving at time <span class="tex-span"><i>t</i> + 1</span> to the same planet.</p><p>Knowing the information about travel times between the planets, and the times when Jack would not be able to use the stargate on particular planets, determine the minimum time in which he can get to the planet with index <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of planets in the galaxy, and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of pairs of planets between which Jack can travel using stargates. Then <span class="tex-span"><i>m</i></span> lines follow, containing three integers each: the <span class="tex-span"><i>i</i></span>-th line contains numbers of planets <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), which are connected through stargates, and the integer transfer time (in seconds) <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) between these planets. It is guaranteed that between any pair of planets there is at most one stargate connection.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) that denotes the number of moments of time when other travellers arrive to the planet with index <span class="tex-span"><i>i</i></span>. Then <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>ij</i></sub> &lt; 10<sup class="upper-index">9</sup></span>) follow, sorted in ascending order. An integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> means that at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> (in seconds) another traveller arrives to the planet <span class="tex-span"><i>i</i></span>. It is guaranteed that the sum of all <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print a single number — the least amount of time Jack needs to get from planet 1 to planet <span class="tex-span"><i>n</i></span>. If Jack can't get to planet <span class="tex-span"><i>n</i></span> in any amount of time, print number -1.</p></div>

## Input

<p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of planets in the galaxy, and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of pairs of planets between which Jack can travel using stargates. Then <span class="tex-span"><i>m</i></span> lines follow, containing three integers each: the <span class="tex-span"><i>i</i></span>-th line contains numbers of planets <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), which are connected through stargates, and the integer transfer time (in seconds) <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) between these planets. It is guaranteed that between any pair of planets there is at most one stargate connection.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) that denotes the number of moments of time when other travellers arrive to the planet with index <span class="tex-span"><i>i</i></span>. Then <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>ij</i></sub> &lt; 10<sup class="upper-index">9</sup></span>) follow, sorted in ascending order. An integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> means that at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>ij</i></sub></span> (in seconds) another traveller arrives to the planet <span class="tex-span"><i>i</i></span>. It is guaranteed that the sum of all <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print a single number — the least amount of time Jack needs to get from planet 1 to planet <span class="tex-span"><i>n</i></span>. If Jack can't get to planet <span class="tex-span"><i>n</i></span> in any amount of time, print number -1.</p>





```input1
4 6
1 2 2
1 3 3
1 4 8
2 3 4
2 4 5
3 4 3
0
1 3
2 3 4
0

```




```input2
3 1
1 2 3
0
1 3
0

```




```output1
7

```




```output2
-1

```



## Note

<p>In the first sample Jack has three ways to go from planet 1. If he moves to planet 4 at once, he spends 8 seconds. If he transfers to planet 3, he spends 3 seconds, but as other travellers arrive to planet 3 at time 3 and 4, he can travel to planet 4 only at time 5, thus spending 8 seconds in total. But if Jack moves to planet 2, and then — to planet 4, then he spends a total of only <span class="tex-span">2 + 5 = 7</span> seconds.</p><p>In the second sample one can't get from planet 1 to planet 3 by moving through stargates.</p>
