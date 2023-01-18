## Description

<div><p>In the evening Polycarp decided to analyze his today's travel expenses on public transport.</p><p>The bus system in the capital of Berland is arranged in such a way that each bus runs along the route between two stops. Each bus has no intermediate stops. So each of the buses continuously runs along the route from one stop to the other and back. There is at most one bus running between a pair of stops.</p><p>Polycarp made <span class="tex-span"><i>n</i></span> trips on buses. About each trip the stop where he started the trip and the the stop where he finished are known. The trips follow in the chronological order in Polycarp's notes.</p><p>It is known that one trip on any bus costs <span class="tex-span"><i>a</i></span> burles. In case when passenger makes a transshipment the cost of trip decreases to <span class="tex-span"><i>b</i></span> burles (<span class="tex-span"><i>b</i> &lt; <i>a</i></span>). A passenger makes a transshipment if the stop on which he boards the bus coincides with the stop where he left the previous bus. Obviously, the first trip can not be made with transshipment.</p><p>For example, if Polycarp made three consecutive trips: "BerBank" <img align="middle" class="tex-formula" src="file://YLf19nVq.png" style="max-width: 100.0%;max-height: 100.0%;"> "University", "University" <img align="middle" class="tex-formula" src="file://n9K9ZkP9.png" style="max-width: 100.0%;max-height: 100.0%;"> "BerMall", "University" <img align="middle" class="tex-formula" src="file://olXGkhWP.png" style="max-width: 100.0%;max-height: 100.0%;"> "BerBank", then he payed <span class="tex-span"><i>a</i> + <i>b</i> + <i>a</i> = 2<i>a</i> + <i>b</i></span> burles. From the BerBank he arrived to the University, where he made transshipment to the other bus and departed to the BerMall. Then he walked to the University and returned to the BerBank by bus.</p><p>Also Polycarp can buy no more than <span class="tex-span"><i>k</i></span> travel cards. Each travel card costs <span class="tex-span"><i>f</i></span> burles. The travel card for a single bus route makes free of charge any trip by this route (in both directions). Once purchased, a travel card can be used any number of times in any direction.</p><p>What is the smallest amount of money Polycarp could have spent today if he can buy no more than <span class="tex-span"><i>k</i></span> travel cards?</p></div><div class="input-specification"><p>The first line contains five integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i>, <i>k</i>, <i>f</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>, <span class="tex-span">1 ≤ <i>b</i> &lt; <i>a</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 300</span>, <span class="tex-span">1 ≤ <i>f</i> ≤ 1000</span>) where:</p><ul> <li> <span class="tex-span"><i>n</i></span> — the number of Polycarp trips, </li><li> <span class="tex-span"><i>a</i></span> — the cost of a regualar single trip, </li><li> <span class="tex-span"><i>b</i></span> — the cost of a trip after a transshipment, </li><li> <span class="tex-span"><i>k</i></span> — the maximum number of travel cards Polycarp can buy, </li><li> <span class="tex-span"><i>f</i></span> — the cost of a single travel card. </li></ul><p>The following <span class="tex-span"><i>n</i></span> lines describe the trips in the chronological order. Each line contains exactly two different words separated by a single space — the name of the start stop and the name of the finish stop of the trip. All names consist of uppercase and lowercase English letters and have lengths between <span class="tex-span">1</span> to <span class="tex-span">20</span> letters inclusive. Uppercase and lowercase letters should be considered different.</p></div><div class="output-specification"><p>Print the smallest amount of money Polycarp could have spent today, if he can purchase no more than <span class="tex-span"><i>k</i></span> travel cards.</p></div>

## Input

<p>The first line contains five integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i>, <i>k</i>, <i>f</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>, <span class="tex-span">1 ≤ <i>b</i> &lt; <i>a</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 300</span>, <span class="tex-span">1 ≤ <i>f</i> ≤ 1000</span>) where:</p><ul> <li> <span class="tex-span"><i>n</i></span> — the number of Polycarp trips, </li><li> <span class="tex-span"><i>a</i></span> — the cost of a regualar single trip, </li><li> <span class="tex-span"><i>b</i></span> — the cost of a trip after a transshipment, </li><li> <span class="tex-span"><i>k</i></span> — the maximum number of travel cards Polycarp can buy, </li><li> <span class="tex-span"><i>f</i></span> — the cost of a single travel card. </li></ul><p>The following <span class="tex-span"><i>n</i></span> lines describe the trips in the chronological order. Each line contains exactly two different words separated by a single space — the name of the start stop and the name of the finish stop of the trip. All names consist of uppercase and lowercase English letters and have lengths between <span class="tex-span">1</span> to <span class="tex-span">20</span> letters inclusive. Uppercase and lowercase letters should be considered different.</p>

## Output

<p>Print the smallest amount of money Polycarp could have spent today, if he can purchase no more than <span class="tex-span"><i>k</i></span> travel cards.</p>





```input1
3 5 3 1 8
BerBank University
University BerMall
University BerBank

```




```input2
4 2 1 300 1000
a A
A aa
aa AA
AA a

```




```output1
11

```




```output2
5

```



## Note

<p>In the first example Polycarp can buy travel card for the route "BerBank <img align="middle" class="tex-formula" src="file://qeJi6mYr.png" style="max-width: 100.0%;max-height: 100.0%;"> University" and spend <span class="tex-span">8</span> burles. Note that his second trip "University" <img align="middle" class="tex-formula" src="file://BoBCEZKi.png" style="max-width: 100.0%;max-height: 100.0%;"> "BerMall" was made after transshipment, so for this trip Polycarp payed <span class="tex-span">3</span> burles. So the minimum total sum equals to <span class="tex-span">8 + 3 = 11</span> burles.</p><p>In the second example it doesn't make sense to buy travel cards. Note that each of Polycarp trip (except the first) was made with transshipment. So the minimum total sum equals to <span class="tex-span">2 + 1 + 1 + 1 = 5</span> burles.</p>
