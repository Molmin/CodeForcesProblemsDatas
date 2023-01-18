## Description

<div><p>Breaking Good is a new video game which a lot of gamers want to have. There is a certain level in the game that is really difficult even for experienced gamers.</p><p>Walter William, the main character of the game, wants to join a gang called Los Hermanos (The Brothers). The gang controls the whole country which consists of <span class="tex-span"><i>n</i></span> cities with <span class="tex-span"><i>m</i></span> bidirectional roads connecting them. There is no road is connecting a city to itself and for any two cities there is at most one road between them. The country is connected, in the other words, it is possible to reach any city from any other city using the given roads. </p><p>The roads aren't all working. There are some roads which need some more work to be performed to be completely functioning.</p><p>The gang is going to rob a bank! The bank is located in city <span class="tex-span">1</span>. As usual, the hardest part is to escape to their headquarters where the police can't get them. The gang's headquarters is in city <span class="tex-span"><i>n</i></span>. To gain the gang's trust, Walter is in charge of this operation, so he came up with a smart plan.</p><p>First of all the path which they are going to use on their way back from city <span class="tex-span">1</span> to their headquarters <span class="tex-span"><i>n</i></span> must be <span class="tex-font-style-underline">as short as possible</span>, since it is important to finish operation as fast as possible.</p><p>Then, gang has to blow up all other roads in country that don't lay on this path, in order to prevent any police reinforcements. In case of non-working road, they don't have to blow up it as it is already malfunctional. </p><p>If the chosen path has some roads that doesn't work they'll have to repair those roads before the operation.</p><p>Walter discovered that there was a lot of paths that satisfied the condition of being shortest possible so he decided to choose among them a path that minimizes the total number of affected roads (both roads that have to be blown up and roads to be repaired).</p><p>Can you help Walter complete his task and gain the gang's trust?</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <img align="middle" class="tex-formula" src="file://MhU9cJG4.png" style="max-width: 100.0%;max-height: 100.0%;">), the number of cities and number of roads respectively.</p><p>In following <span class="tex-span"><i>m</i></span> lines there are descriptions of roads. Each description consists of three integers <span class="tex-span"><i>x</i>, <i>y</i>, <i>z</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <img align="middle" class="tex-formula" src="file://UtH0UNMn.png" style="max-width: 100.0%;max-height: 100.0%;">) meaning that there is a road connecting cities number <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. If <span class="tex-span"><i>z</i> = 1</span>, this road is working, otherwise it is not.</p></div><div class="output-specification"><p>In the first line output one integer <span class="tex-span"><i>k</i></span>, the minimum possible number of roads affected by gang.</p><p>In the following <span class="tex-span"><i>k</i></span> lines output three integers describing roads that should be affected. Each line should contain three integers <span class="tex-span"><i>x</i>, <i>y</i>, <i>z</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <img align="middle" class="tex-formula" src="file://d78vwFU2.png" style="max-width: 100.0%;max-height: 100.0%;">), cities connected by a road and the new state of a road. <span class="tex-span"><i>z</i> = 1</span> indicates that the road between cities <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> should be repaired and <span class="tex-span"><i>z</i> = 0</span> means that road should be blown up. </p><p>You may output roads in any order. Each affected road should appear exactly once. You may output cities connected by a single road in any order. If you output a road, it's original state should be different from <span class="tex-span"><i>z</i></span>.</p><p>After performing all operations accroding to your plan, there should remain working only roads lying on some certain shortest past between city <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>.</p><p>If there are multiple optimal answers output any.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <img align="middle" class="tex-formula" src="file://MhU9cJG4.png" style="max-width: 100.0%;max-height: 100.0%;">), the number of cities and number of roads respectively.</p><p>In following <span class="tex-span"><i>m</i></span> lines there are descriptions of roads. Each description consists of three integers <span class="tex-span"><i>x</i>, <i>y</i>, <i>z</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <img align="middle" class="tex-formula" src="file://UtH0UNMn.png" style="max-width: 100.0%;max-height: 100.0%;">) meaning that there is a road connecting cities number <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. If <span class="tex-span"><i>z</i> = 1</span>, this road is working, otherwise it is not.</p>

## Output

<p>In the first line output one integer <span class="tex-span"><i>k</i></span>, the minimum possible number of roads affected by gang.</p><p>In the following <span class="tex-span"><i>k</i></span> lines output three integers describing roads that should be affected. Each line should contain three integers <span class="tex-span"><i>x</i>, <i>y</i>, <i>z</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <img align="middle" class="tex-formula" src="file://d78vwFU2.png" style="max-width: 100.0%;max-height: 100.0%;">), cities connected by a road and the new state of a road. <span class="tex-span"><i>z</i> = 1</span> indicates that the road between cities <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> should be repaired and <span class="tex-span"><i>z</i> = 0</span> means that road should be blown up. </p><p>You may output roads in any order. Each affected road should appear exactly once. You may output cities connected by a single road in any order. If you output a road, it's original state should be different from <span class="tex-span"><i>z</i></span>.</p><p>After performing all operations accroding to your plan, there should remain working only roads lying on some certain shortest past between city <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>.</p><p>If there are multiple optimal answers output any.</p>





```input1
2 1
1 2 0

```




```input2
4 4
1 2 1
1 3 0
2 3 1
3 4 1

```




```input3
8 9
1 2 0
8 3 0
2 3 1
1 4 1
8 7 0
1 5 1
4 6 1
5 7 0
6 8 0

```




```output1
1
1 2 1

```




```output2
3
1 2 0
1 3 1
2 3 0

```




```output3
3
2 3 0
1 5 0
6 8 1

```



## Note

<p>In the first test the only path is <span class="tex-span">1 - 2</span></p><p>In the second test the only shortest path is <span class="tex-span">1 - 3 - 4</span></p><p>In the third test there are multiple shortest paths but the optimal is <span class="tex-span">1 - 4 - 6 - 8</span></p>
