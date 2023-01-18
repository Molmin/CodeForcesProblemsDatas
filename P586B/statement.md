## Description

<div><p>A little boy Laurenty has been playing his favourite game <span class="tex-font-style-tt">Nota</span> for quite a while and is now very hungry. The boy wants to make sausage and cheese sandwiches, but first, he needs to buy a sausage and some cheese.</p><p>The town where Laurenty lives in is not large. The houses in it are located in two rows, <span class="tex-span"><i>n</i></span> houses in each row. Laurenty lives in the very last house of the second row. The only shop in town is placed in the first house of the first row.</p><p>The first and second rows are separated with the main avenue of the city. The adjacent houses of one row are separated by streets.</p><p>Each crosswalk of a street or an avenue has some traffic lights. In order to cross the street, you need to press a button on the traffic light, wait for a while for the green light and cross the street. Different traffic lights can have different waiting time.</p><p>The traffic light on the crosswalk from the <span class="tex-span"><i>j</i></span>-th house of the <span class="tex-span"><i>i</i></span>-th row to the <span class="tex-span">(<i>j</i> + 1)</span>-th house of the same row has waiting time equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ 2, 1 ≤ <i>j</i> ≤ <i>n</i> - 1</span>). For the traffic light on the crossing from the <span class="tex-span"><i>j</i></span>-th house of one row to the <span class="tex-span"><i>j</i></span>-th house of another row the waiting time equals <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>). The city doesn't have any other crossings.</p><p>The boy wants to get to the store, buy the products and go back. The main avenue of the city is wide enough, so the boy wants to cross it <span class="tex-font-style-bf">exactly once</span> on the way to the store and <span class="tex-font-style-bf">exactly once</span> on the way back home. The boy would get bored if he had to walk the same way again, so he wants the way home to be different from the way to the store in at least one crossing.</p><center> <img class="tex-graphics" src="file://ANqiNcyk.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Figure to the first sample.</span> </center><p>Help Laurenty determine the minimum total time he needs to wait at the crossroads.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>) — the number of houses in each row. </p><p>Each of the next two lines contains <span class="tex-span"><i>n</i> - 1</span> space-separated integer — values <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 100</span>). </p><p>The last line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>Print a single integer — the least total time Laurenty needs to wait at the crossroads, given that he crosses the avenue only once both on his way to the store and on his way back home.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>) — the number of houses in each row. </p><p>Each of the next two lines contains <span class="tex-span"><i>n</i> - 1</span> space-separated integer — values <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 100</span>). </p><p>The last line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 100</span>).</p>

## Output

<p>Print a single integer — the least total time Laurenty needs to wait at the crossroads, given that he crosses the avenue only once both on his way to the store and on his way back home.</p>





```input1
4
1 2 3
3 2 1
3 2 2 3

```




```input2
3
1 2
3 3
2 1 3

```




```input3
2
1
1
1 1

```




```output1
12

```




```output2
11

```




```output3
4

```



## Note

<p>The first sample is shown on the figure above. </p><p>In the second sample, Laurenty's path can look as follows: </p><ul> <li> Laurenty crosses the avenue, the waiting time is <span class="tex-span">3</span>; </li><li> Laurenty uses the second crossing in the first row, the waiting time is <span class="tex-span">2</span>; </li><li> Laurenty uses the first crossing in the first row, the waiting time is <span class="tex-span">1</span>; </li><li> Laurenty uses the first crossing in the first row, the waiting time is <span class="tex-span">1</span>; </li><li> Laurenty crosses the avenue, the waiting time is <span class="tex-span">1</span>; </li><li> Laurenty uses the second crossing in the second row, the waiting time is <span class="tex-span">3</span>. </li></ul> In total we get that the answer equals <span class="tex-span">11</span>.<p>In the last sample Laurenty visits all the crossings, so the answer is <span class="tex-span">4</span>.</p>
