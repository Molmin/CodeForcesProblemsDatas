## Description

<div><p>Musicians of a popular band "Flayer" have announced that they are going to "make their exit" with a world tour. Of course, they will visit Berland as well.</p><p>There are <span class="tex-span"><i>n</i></span> cities in Berland. People can travel between cities using two-directional train routes; there are exactly <span class="tex-span"><i>m</i></span> routes, <span class="tex-span"><i>i</i></span>-th route can be used to go from city <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (and from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>), and it costs <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> coins to use this route.</p><p>Each city will be visited by "Flayer", and the cost of the concert ticket in <span class="tex-span"><i>i</i></span>-th city is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> coins.</p><p>You have friends in every city of Berland, and they, knowing about your programming skills, asked you to calculate the minimum possible number of coins they have to pay to visit the concert. For every city <span class="tex-span"><i>i</i></span> you have to compute the minimum number of coins a person from city <span class="tex-span"><i>i</i></span> has to spend to travel to some city <span class="tex-span"><i>j</i></span> (or possibly stay in city <span class="tex-span"><i>i</i></span>), attend a concert there, and return to city <span class="tex-span"><i>i</i></span> (if <span class="tex-span"><i>j</i> ≠ <i>i</i></span>).</p><p>Formally, for every <img align="middle" class="tex-formula" src="file://FCGsdJZS.png" style="max-width: 100.0%;max-height: 100.0%;"> you have to calculate <img align="middle" class="tex-formula" src="file://ltDAVQNt.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>d</i>(<i>i</i>, <i>j</i>)</span> is the minimum number of coins you have to spend to travel from city <span class="tex-span"><i>i</i></span> to city <span class="tex-span"><i>j</i></span>. If there is no way to reach city <span class="tex-span"><i>j</i></span> from city <span class="tex-span"><i>i</i></span>, then we consider <span class="tex-span"><i>d</i>(<i>i</i>, <i>j</i>)</span> to be infinitely large.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th contains three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) denoting <span class="tex-span"><i>i</i></span>-th train route. There are no multiple train routes connecting the same pair of cities, that is, for each <span class="tex-span">(<i>v</i>, <i>u</i>)</span> neither extra <span class="tex-span">(<i>v</i>, <i>u</i>)</span> nor <span class="tex-span">(<i>u</i>, <i>v</i>)</span> present in input.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) — price to attend the concert in <span class="tex-span"><i>i</i></span>-th city.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them must be equal to the minimum number of coins a person from city <span class="tex-span"><i>i</i></span> has to spend to travel to some city <span class="tex-span"><i>j</i></span> (or possibly stay in city <span class="tex-span"><i>i</i></span>), attend a concert there, and return to city <span class="tex-span"><i>i</i></span> (if <span class="tex-span"><i>j</i> ≠ <i>i</i></span>).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th contains three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) denoting <span class="tex-span"><i>i</i></span>-th train route. There are no multiple train routes connecting the same pair of cities, that is, for each <span class="tex-span">(<i>v</i>, <i>u</i>)</span> neither extra <span class="tex-span">(<i>v</i>, <i>u</i>)</span> nor <span class="tex-span">(<i>u</i>, <i>v</i>)</span> present in input.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) — price to attend the concert in <span class="tex-span"><i>i</i></span>-th city.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them must be equal to the minimum number of coins a person from city <span class="tex-span"><i>i</i></span> has to spend to travel to some city <span class="tex-span"><i>j</i></span> (or possibly stay in city <span class="tex-span"><i>i</i></span>), attend a concert there, and return to city <span class="tex-span"><i>i</i></span> (if <span class="tex-span"><i>j</i> ≠ <i>i</i></span>).</p>





```input1
4 2
1 2 4
2 3 7
6 20 1 25

```




```input2
3 3
1 2 1
2 3 1
1 3 1
30 10 20

```




```output1
6 14 1 25 

```




```output2
12 10 12 

```


