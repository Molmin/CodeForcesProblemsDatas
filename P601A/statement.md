## Description

<div><p>In Absurdistan, there are <span class="tex-span"><i>n</i></span> towns (numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>) and <span class="tex-span"><i>m</i></span> bidirectional railways. There is also an absurdly simple road network&nbsp;— for each pair of different towns <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, there is a bidirectional road between towns <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-font-style-bf">if and only if</span> there is no railway between them. Travelling to a different town using one railway or one road always takes exactly one hour.</p><p>A train and a bus leave town <span class="tex-span">1</span> at the same time. They both have the same destination, town <span class="tex-span"><i>n</i></span>, and don't make any stops on the way (but they can wait in town <span class="tex-span"><i>n</i></span>). The train can move only along railways and the bus can move only along roads.</p><p>You've been asked to plan out routes for the vehicles; each route can use any road/railway multiple times. One of the most important aspects to consider is safety&nbsp;— in order to avoid accidents at railway crossings, the train and the bus must not arrive at the same town (except town <span class="tex-span"><i>n</i></span>) simultaneously.</p><p>Under these constraints, what is the minimum number of hours needed for both vehicles to reach town <span class="tex-span"><i>n</i></span> (the maximum of arrival times of the bus and the train)? Note, that bus and train are not required to arrive to the town <span class="tex-span"><i>n</i></span> at the same moment of time, but are allowed to do so.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i>(<i>n</i> - 1) / 2</span>)&nbsp;— the number of towns and the number of railways respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, denoting a railway between towns <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>).</p><p>You may assume that there is at most one railway connecting any two towns.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the smallest possible time of the later vehicle's arrival in town <span class="tex-span"><i>n</i></span>. If it's impossible for at least one of the vehicles to reach town <span class="tex-span"><i>n</i></span>, output <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i>(<i>n</i> - 1) / 2</span>)&nbsp;— the number of towns and the number of railways respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, denoting a railway between towns <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>).</p><p>You may assume that there is at most one railway connecting any two towns.</p>

## Output

<p>Output one integer&nbsp;— the smallest possible time of the later vehicle's arrival in town <span class="tex-span"><i>n</i></span>. If it's impossible for at least one of the vehicles to reach town <span class="tex-span"><i>n</i></span>, output <span class="tex-span"> - 1</span>.</p>





```input1
4 2
1 3
3 4

```




```input2
4 6
1 2
1 3
1 4
2 3
2 4
3 4

```




```input3
5 5
4 2
3 5
4 5
5 1
1 2

```




```output1
2

```




```output2
-1

```




```output3
3

```



## Note

<p>In the first sample, the train can take the route <img align="middle" class="tex-formula" src="file://8NT0xX8c.png" style="max-width: 100.0%;max-height: 100.0%;"> and the bus can take the route <img align="middle" class="tex-formula" src="file://W7NSEcqe.png" style="max-width: 100.0%;max-height: 100.0%;">. Note that they can arrive at town <span class="tex-span">4</span> at the same time.</p><p>In the second sample, Absurdistan is ruled by railwaymen. There are no roads, so there's no way for the bus to reach town <span class="tex-span">4</span>.</p>
