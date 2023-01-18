## Description

<div><p>The Berland capital (as you very well know) contains <span class="tex-span"><i>n</i></span> junctions, some pairs of which are connected by two-way roads. Unfortunately, the number of traffic jams in the capital has increased dramatically, that's why it was decided to build several new roads. Every road should connect two junctions. </p><p>The city administration noticed that in the cities of all the developed countries between any two roads one can drive along at least two paths so that the paths don't share any roads (but they may share the same junction). The administration decided to add the minimal number of roads so that this rules was fulfilled in the Berland capital as well. In the city road network should exist no more than one road between every pair of junctions before or after the reform.</p></div><div class="input-specification"><p>The first input line contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 900, 1 ≤ <i>m</i> ≤ 100000</span>), where <span class="tex-span"><i>n</i></span> is the number of junctions and <span class="tex-span"><i>m</i></span> is the number of roads. Each of the following <span class="tex-span"><i>m</i></span> lines contains a description of a road that is given by the numbers of the connected junctions <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). The junctions are numbered from 1 to <span class="tex-span"><i>n</i></span>. It is possible to reach any junction of the city from any other one moving along roads.</p></div><div class="output-specification"><p>On the first line print <span class="tex-span"><i>t</i></span> — the number of added roads. Then on <span class="tex-span"><i>t</i></span> lines print the descriptions of the added roads in the format of the input data. You can use any order of printing the roads themselves as well as the junctions linked by every road. If there are several solutions to that problem, print any of them.</p><p>If the capital doesn't need the reform, print the single number <span class="tex-font-style-tt">0</span>.</p><p>If there's no solution, print the single number <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first input line contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 900, 1 ≤ <i>m</i> ≤ 100000</span>), where <span class="tex-span"><i>n</i></span> is the number of junctions and <span class="tex-span"><i>m</i></span> is the number of roads. Each of the following <span class="tex-span"><i>m</i></span> lines contains a description of a road that is given by the numbers of the connected junctions <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). The junctions are numbered from 1 to <span class="tex-span"><i>n</i></span>. It is possible to reach any junction of the city from any other one moving along roads.</p>

## Output

<p>On the first line print <span class="tex-span"><i>t</i></span> — the number of added roads. Then on <span class="tex-span"><i>t</i></span> lines print the descriptions of the added roads in the format of the input data. You can use any order of printing the roads themselves as well as the junctions linked by every road. If there are several solutions to that problem, print any of them.</p><p>If the capital doesn't need the reform, print the single number <span class="tex-font-style-tt">0</span>.</p><p>If there's no solution, print the single number <span class="tex-font-style-tt">-1</span>.</p>





```input1
4 3
1 2
2 3
3 4

```




```input2
4 4
1 2
2 3
2 4
3 4

```




```output1
1
1 4

```




```output2
1
1 3

```


