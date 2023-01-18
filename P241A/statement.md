## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities in the country where the Old Peykan lives. These cities are located on a straight line, we'll denote them from left to right as <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>. The Old Peykan wants to travel from city <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span> using roads. There are <span class="tex-span">(<i>n</i> - 1)</span> <span class="tex-font-style-bf">one way</span> roads, the <span class="tex-span"><i>i</i></span>-th road goes from city <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> and is <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> kilometers long.</p><p>The Old Peykan travels 1 kilometer in 1 hour and consumes 1 liter of fuel during this time.</p><p>Each city <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (except for the last city <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span>) has a supply of <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> liters of fuel which immediately transfers to the Old Peykan if it passes the city or stays in it. This supply refreshes instantly <span class="tex-span"><i>k</i></span> hours after it transfers. The Old Peykan can stay in a city for a while and fill its fuel tank many times. </p><p>Initially (at time zero) the Old Peykan is at city <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> liters of fuel is transferred to it's empty tank from <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>'s supply. The Old Peykan's fuel tank capacity is unlimited. Old Peykan can not continue its travel if its tank is emptied strictly between two cities.</p><p>Find the minimum time the Old Peykan needs to reach city <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span>.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>m</i>, <i>k</i> ≤ 1000)</span>. The value <span class="tex-span"><i>m</i></span> specifies the number of roads between cities which is equal to <span class="tex-span"><i>n</i> - 1</span>.</p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> and the following line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>.</p></div><div class="output-specification"><p>In the only line of the output print a single integer — the minimum time required for The Old Peykan to reach city <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span> from city <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>m</i>, <i>k</i> ≤ 1000)</span>. The value <span class="tex-span"><i>m</i></span> specifies the number of roads between cities which is equal to <span class="tex-span"><i>n</i> - 1</span>.</p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> and the following line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>.</p>

## Output

<p>In the only line of the output print a single integer — the minimum time required for The Old Peykan to reach city <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span> from city <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>.</p>





```input1
4 6
1 2 5 2
2 3 3 4

```




```input2
2 3
5 6
5 5

```




```output1
10

```




```output2
14

```



## Note

<p>In the second sample above, the Old Peykan stays in <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> for 3 hours.</p>
