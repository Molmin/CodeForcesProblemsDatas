## Description

<div><p>In the country of Never, there are <span class="tex-span"><i>n</i></span> cities and a well-developed road system. There is exactly one bidirectional road between every pair of cities, thus, there are as many as <img align="middle" class="tex-formula" src="file://qf3AGhna.png" style="max-width: 100.0%;max-height: 100.0%;"> roads! No two roads intersect, and no road passes through intermediate cities. The art of building tunnels and bridges has been mastered by Neverians.</p><p>An independent committee has evaluated each road of Never with a positive integer called the <span class="tex-font-style-underline">perishability</span> of the road. The lower the road's perishability is, the more pleasant it is to drive through this road.</p><p>It's the year of transport in Never. It has been decided to build a museum of transport in one of the cities, and to set a single signpost directing to some city (not necessarily the one with the museum) in each of the other cities. The signposts must satisfy the following important condition: if any Neverian living in a city without the museum starts travelling from that city following the directions of the signposts, then this person will eventually arrive in the city with the museum.</p><p>Neverians are incredibly positive-minded. If a Neverian travels by a route consisting of several roads, he considers the <span class="tex-font-style-underline">perishability of the route</span> to be equal to the smallest perishability of all the roads in this route.</p><p>The government of Never has not yet decided where to build the museum, so they consider all <span class="tex-span"><i>n</i></span> possible options. The most important is the sum of perishabilities of the routes to the museum city from all the other cities of Never, if the travelers strictly follow the directions of the signposts. The government of Never cares about their citizens, so they want to set the signposts in a way which minimizes this sum. Help them determine the minimum possible sum for all <span class="tex-span"><i>n</i></span> possible options of the city where the museum can be built.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the number of cities in Never.</p><p>The following <span class="tex-span"><i>n</i> - 1</span> lines contain the description of the road network. The <span class="tex-span"><i>i</i></span>-th of these lines contains <span class="tex-span"><i>n</i> - <i>i</i></span> integers. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line denotes the perishability of the road between cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + <i>j</i></span>.</p><p>All road perishabilities are between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive.</p></div><div class="output-specification"><p>For each city in order from 1 to <span class="tex-span"><i>n</i></span>, output the minimum possible sum of perishabilities of the routes to this city from all the other cities of Never if the signposts are set in a way which minimizes this sum.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the number of cities in Never.</p><p>The following <span class="tex-span"><i>n</i> - 1</span> lines contain the description of the road network. The <span class="tex-span"><i>i</i></span>-th of these lines contains <span class="tex-span"><i>n</i> - <i>i</i></span> integers. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line denotes the perishability of the road between cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + <i>j</i></span>.</p><p>All road perishabilities are between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive.</p>

## Output

<p>For each city in order from 1 to <span class="tex-span"><i>n</i></span>, output the minimum possible sum of perishabilities of the routes to this city from all the other cities of Never if the signposts are set in a way which minimizes this sum.</p>





```input1
3
1 2
3

```




```input2
6
2 9 9 6 6
7 1 9 10
9 2 5
4 10
8

```




```output1
2
2
3

```




```output2
6
5
7
5
7
11

```



## Note

<p>The first example is explained by the picture below. From left to right, there is the initial road network and the optimal directions of the signposts in case the museum is built in city 1, 2 and 3, respectively. The museum city is represented by a blue circle, the directions of the signposts are represented by green arrows.</p><p>For instance, if the museum is built in city 3, then the signpost in city 1 must be directed to city 3, while the signpost in city 2 must be directed to city 1. Then the route from city 1 to city 3 will have perishability 2, while the route from city 2 to city 3 will have perishability 1. The sum of perishabilities of these routes is 3.</p><center> <img class="tex-graphics" src="file://nMjHcKyr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
