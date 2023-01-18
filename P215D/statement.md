## Description

<div><p>The official capital and the cultural capital of Berland are connected by a single road running through <span class="tex-span"><i>n</i></span> regions. Each region has a unique climate, so the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> region has a stable temperature of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> degrees in summer.</p><p>This summer a group of <span class="tex-span"><i>m</i></span> schoolchildren wants to get from the official capital to the cultural capital to visit museums and sights. The trip organizers transport the children between the cities in buses, but sometimes it is very hot. Specifically, if the bus is driving through the <span class="tex-span"><i>i</i></span>-th region and has <span class="tex-span"><i>k</i></span> schoolchildren, then the temperature inside the bus is <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> + <i>k</i></span> degrees.</p><p>Of course, nobody likes it when the bus is hot. So, when the bus drives through the <span class="tex-span"><i>i</i></span>-th region, if it has more than <span class="tex-span"><i>T</i><sub class="lower-index"><i>i</i></sub></span> degrees inside, each of the schoolchild in the bus demands compensation for the uncomfortable conditions. The compensation is as large as <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> rubles and it is charged in each region where the temperature in the bus exceeds the limit.</p><p>To save money, the organizers of the trip may arbitrarily add or remove extra buses in the beginning of the trip, and between regions (of course, they need at least one bus to pass any region). The organizers can also arbitrarily sort the children into buses, however, each of buses in the <span class="tex-span"><i>i</i></span>-th region will cost the organizers <span class="tex-span"><i>cost</i><sub class="lower-index"><i>i</i></sub></span> rubles. Please note that sorting children into buses takes no money.</p><p>Your task is to find the minimum number of rubles, which the organizers will have to spend to transport all schoolchildren.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>;&nbsp;<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of regions on the way and the number of schoolchildren in the group, correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain four integers each: the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>T</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>cost</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>T</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>cost</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print the only integer — the minimum number of roubles the organizers will have to spend to transport all schoolchildren.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>;&nbsp;<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of regions on the way and the number of schoolchildren in the group, correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain four integers each: the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>T</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>cost</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>T</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>cost</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). The numbers in the lines are separated by single spaces.</p>

## Output

<p>Print the only integer — the minimum number of roubles the organizers will have to spend to transport all schoolchildren.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
2 10
30 35 1 100
20 35 10 10

```




```input2
3 100
10 30 1000 1
5 10 1000 3
10 40 1000 100000

```




```output1
120

```




```output2
200065

```



## Note

<p>In the first sample the organizers will use only one bus to travel through the first region. However, the temperature in the bus will equal <span class="tex-span">30 + 10 = 40</span> degrees and each of <span class="tex-span">10</span> schoolchildren will ask for compensation. Only one bus will transport the group through the second region too, but the temperature inside won't exceed the limit. Overall, the organizers will spend <span class="tex-span">100 + 10 + 10 = 120</span> rubles.</p>
