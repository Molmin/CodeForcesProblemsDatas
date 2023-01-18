## Description

<div><p>Bajtek is learning to skate on ice. He's a beginner, so his only mode of transportation is pushing off from a snow drift to the north, east, south or west and sliding until he lands in another snow drift. He has noticed that in this way it's impossible to get from some snow drifts to some other by any sequence of moves. He now wants to heap up some additional snow drifts, so that he can get from any snow drift to any other one. He asked you to find the minimal number of snow drifts that need to be created.</p><p>We assume that Bajtek can only heap up snow drifts at integer coordinates.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of snow drifts. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th snow drift.</p><p>Note that the north direction coinсides with the direction of <span class="tex-span"><i>Oy</i></span> axis, so the east direction coinсides with the direction of the <span class="tex-span"><i>Ox</i></span> axis. All snow drift's locations are distinct.</p></div><div class="output-specification"><p>Output the minimal number of snow drifts that need to be created in order for Bajtek to be able to reach any snow drift from any other one.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of snow drifts. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th snow drift.</p><p>Note that the north direction coinсides with the direction of <span class="tex-span"><i>Oy</i></span> axis, so the east direction coinсides with the direction of the <span class="tex-span"><i>Ox</i></span> axis. All snow drift's locations are distinct.</p>

## Output

<p>Output the minimal number of snow drifts that need to be created in order for Bajtek to be able to reach any snow drift from any other one.</p>





```input1
2
2 1
1 2

```




```input2
2
2 1
4 1

```




```output1
1

```




```output2
0

```


