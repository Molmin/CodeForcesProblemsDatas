## Description

<div><p>Berland Government decided to improve relations with neighboring countries. First of all, it was decided to build new roads so that from each city of Berland and neighboring countries it became possible to reach all the others. There are <span class="tex-span"><i>n</i></span> cities in Berland and neighboring countries in total and exactly <span class="tex-span"><i>n</i> - 1</span> two-way roads. Because of the recent financial crisis, the Berland Government is strongly pressed for money, so to build a new road it has to close some of the existing ones. Every day it is possible to close one existing road and immediately build a new one. Your task is to determine how many days would be needed to rebuild roads so that from each city it became possible to reach all the others, and to draw a plan of closure of old roads and building of new ones.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — amount of cities in Berland and neighboring countries. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the description of roads. Each road is described by two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — pair of cities, which the road connects. It can't be more than one road between a pair of cities. No road connects the city with itself.</p></div><div class="output-specification"><p>Output the answer, number <span class="tex-span"><i>t</i></span> — what is the least amount of days needed to rebuild roads so that from each city it became possible to reach all the others. Then output <span class="tex-span"><i>t</i></span> lines — the plan of closure of old roads and building of new ones. Each line should describe one day in the format <span class="tex-font-style-tt">i j u v</span> — it means that road between cities <span class="tex-font-style-tt">i</span> and <span class="tex-font-style-tt">j</span> became closed and a new road between cities <span class="tex-font-style-tt">u</span> and <span class="tex-font-style-tt">v</span> is built. Cities are numbered from 1. If the answer is not unique, output any.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — amount of cities in Berland and neighboring countries. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the description of roads. Each road is described by two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — pair of cities, which the road connects. It can't be more than one road between a pair of cities. No road connects the city with itself.</p>

## Output

<p>Output the answer, number <span class="tex-span"><i>t</i></span> — what is the least amount of days needed to rebuild roads so that from each city it became possible to reach all the others. Then output <span class="tex-span"><i>t</i></span> lines — the plan of closure of old roads and building of new ones. Each line should describe one day in the format <span class="tex-font-style-tt">i j u v</span> — it means that road between cities <span class="tex-font-style-tt">i</span> and <span class="tex-font-style-tt">j</span> became closed and a new road between cities <span class="tex-font-style-tt">u</span> and <span class="tex-font-style-tt">v</span> is built. Cities are numbered from 1. If the answer is not unique, output any.</p>





```input1
2
1 2

```




```input2
7
1 2
2 3
3 1
4 5
5 6
6 7

```




```output1
0

```




```output2
1
3 1 3 7

```


