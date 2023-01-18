## Description

<div><p>Friends Alex and Bob live in Bertown. In this town there are <span class="tex-span"><i>n</i></span> crossroads, some of them are connected by bidirectional roads of equal length. Bob lives in a house at the crossroads number <span class="tex-span">1</span>, Alex — in a house at the crossroads number <span class="tex-span"><i>n</i></span>.</p><p>One day Alex and Bob had a big quarrel, and they refused to see each other. It occurred that today Bob needs to get from his house to the crossroads <span class="tex-span"><i>n</i></span> and Alex needs to get from his house to the crossroads <span class="tex-span">1</span>. And they don't want to meet at any of the crossroads, but they can meet in the middle of the street, when passing it in opposite directions. Alex and Bob asked you, as their mutual friend, to help them with this difficult task.</p><p>Find for Alex and Bob such routes with equal number of streets that the guys can follow these routes and never appear at the same crossroads at the same time. They are allowed to meet in the middle of the street when moving toward each other (see Sample 1). Among all possible routes, select such that the number of streets in it is the least possible. Until both guys reach their destinations, none of them can stay without moving. </p><p>The guys are moving simultaneously with equal speeds, i.e. it is possible that when one of them reaches some of the crossroads, the other one leaves it. For example, Alex can move from crossroad <span class="tex-span">1</span> to crossroad <span class="tex-span">2</span>, while Bob moves from crossroad <span class="tex-span">2</span> to crossroad <span class="tex-span">3</span>.</p><p>If the required routes don't exist, your program should output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500, 1 ≤ <i>m</i> ≤ 10000</span>) — the amount of crossroads and the amount of roads. Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers — the numbers of crossroads connected by the road. It is guaranteed that no road connects a crossroads with itself and no two crossroads are connected by more than one road.</p></div><div class="output-specification"><p>If the required routes don't exist, output <span class="tex-font-style-tt">-1</span>. Otherwise, the first line should contain integer <span class="tex-span"><i>k</i></span> — the length of shortest routes (the length of the route is the amount of roads in it). The next line should contain <span class="tex-span"><i>k</i> + 1</span> integers — Bob's route, i.e. the numbers of <span class="tex-span"><i>k</i> + 1</span> crossroads passed by Bob. The last line should contain Alex's route in the same format. If there are several optimal solutions, output any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500, 1 ≤ <i>m</i> ≤ 10000</span>) — the amount of crossroads and the amount of roads. Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers — the numbers of crossroads connected by the road. It is guaranteed that no road connects a crossroads with itself and no two crossroads are connected by more than one road.</p>

## Output

<p>If the required routes don't exist, output <span class="tex-font-style-tt">-1</span>. Otherwise, the first line should contain integer <span class="tex-span"><i>k</i></span> — the length of shortest routes (the length of the route is the amount of roads in it). The next line should contain <span class="tex-span"><i>k</i> + 1</span> integers — Bob's route, i.e. the numbers of <span class="tex-span"><i>k</i> + 1</span> crossroads passed by Bob. The last line should contain Alex's route in the same format. If there are several optimal solutions, output any of them.</p>





```input1
2 1
1 2

```




```input2
7 5
1 2
2 7
7 6
2 3
3 4

```




```input3
7 6
1 2
2 7
7 6
2 3
3 4
1 5

```




```output1
1
1 2 
2 1 

```




```output2
-1

```




```output3
6
1 2 3 4 3 2 7 
7 6 7 2 1 5 1 

```


