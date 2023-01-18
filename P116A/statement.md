## Description

<div><p>Linear Kingdom has exactly one tram line. It has <span class="tex-span"><i>n</i></span> stops, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order of tram's movement. At the <span class="tex-span"><i>i</i></span>-th stop <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> passengers exit the tram, while <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> passengers enter it. The tram is empty before it arrives at the first stop. Also, when the tram arrives at the last stop, all passengers exit so that it becomes empty.</p><p>Your task is to calculate the tram's minimum capacity such that the number of people inside the tram at any time never exceeds this capacity. Note that at each stop all exiting passengers exit <span class="tex-font-style-bf">before</span> any entering passenger enters the tram.</p></div><div class="input-specification"><p>The first line contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — the number of the tram's stops. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the number of passengers that exits the tram at the <span class="tex-span"><i>i</i></span>-th stop, and the number of passengers that enter the tram at the <span class="tex-span"><i>i</i></span>-th stop. The stops are given from the first to the last stop in the order of tram's movement.</p><ul> <li> The number of people who exit at a given stop does not exceed the total number of people in the tram immediately before it arrives at the stop. More formally, <img align="middle" class="tex-formula" src="file://7p6DdIw3.png" style="max-width: 100.0%;max-height: 100.0%;">. This particularly means that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 0</span>. </li><li> At the last stop, <span class="tex-font-style-bf">all</span> the passengers exit the tram and it becomes empty. More formally, <img align="middle" class="tex-formula" src="file://WpJqnYp1.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> No passenger will enter the train at the last stop. That is, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub> = 0</span>. </li></ul></div><div class="output-specification"><p>Print a single integer denoting the minimum possible capacity of the tram (0 is allowed).</p></div>

## Input

<p>The first line contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — the number of the tram's stops. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the number of passengers that exits the tram at the <span class="tex-span"><i>i</i></span>-th stop, and the number of passengers that enter the tram at the <span class="tex-span"><i>i</i></span>-th stop. The stops are given from the first to the last stop in the order of tram's movement.</p><ul> <li> The number of people who exit at a given stop does not exceed the total number of people in the tram immediately before it arrives at the stop. More formally, <img align="middle" class="tex-formula" src="file://7p6DdIw3.png" style="max-width: 100.0%;max-height: 100.0%;">. This particularly means that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 0</span>. </li><li> At the last stop, <span class="tex-font-style-bf">all</span> the passengers exit the tram and it becomes empty. More formally, <img align="middle" class="tex-formula" src="file://WpJqnYp1.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> No passenger will enter the train at the last stop. That is, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub> = 0</span>. </li></ul>

## Output

<p>Print a single integer denoting the minimum possible capacity of the tram (0 is allowed).</p>





```input1
4
0 3
2 5
4 2
4 0

```




```output1
6

```



## Note

<p>For the first example, a capacity of 6 is sufficient: </p><ul> <li> At the first stop, the number of passengers inside the tram before arriving is 0. Then, 3 passengers enter the tram, and the number of passengers inside the tram becomes 3. </li><li> At the second stop, 2 passengers exit the tram (1 passenger remains inside). Then, 5 passengers enter the tram. There are 6 passengers inside the tram now. </li><li> At the third stop, 4 passengers exit the tram (2 passengers remain inside). Then, 2 passengers enter the tram. There are 4 passengers inside the tram now. </li><li> Finally, all the remaining passengers inside the tram exit the tram at the last stop. There are no passenger inside the tram now, which is in line with the constraints. </li></ul><p>Since the number of passengers inside the tram never exceeds 6, a capacity of 6 is sufficient. Furthermore it is not possible for the tram to have a capacity less than 6. Hence, 6 is the correct answer.</p>
