## Description

<div><p>Nowadays the one-way traffic is introduced all over the world in order to improve driving safety and reduce traffic jams. The government of Berland decided to keep up with new trends. Formerly all <span class="tex-span"><i>n</i></span> cities of Berland were connected by <span class="tex-span"><i>n</i></span> two-way roads in the ring, i. e. each city was connected directly to exactly two other cities, and from each city it was possible to get to any other city. Government of Berland introduced one-way traffic on all <span class="tex-span"><i>n</i></span> roads, but it soon became clear that it's impossible to get from some of the cities to some others. Now for each road is known in which direction the traffic is directed at it, and the cost of redirecting the traffic. What is the smallest amount of money the government should spend on the redirecting of roads so that from every city you can get to any other?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — amount of cities (and roads) in Berland. Next <span class="tex-span"><i>n</i></span> lines contain description of roads. Each road is described by three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — road is directed from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, redirecting the traffic costs <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Output single integer — the smallest amount of money the government should spend on the redirecting of roads so that from every city you can get to any other.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — amount of cities (and roads) in Berland. Next <span class="tex-span"><i>n</i></span> lines contain description of roads. Each road is described by three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — road is directed from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, redirecting the traffic costs <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Output single integer — the smallest amount of money the government should spend on the redirecting of roads so that from every city you can get to any other.</p>





```input1
3
1 3 1
1 2 1
3 2 1

```




```input2
3
1 3 1
1 2 5
3 2 1

```




```input3
6
1 5 4
5 3 8
2 4 15
1 6 16
2 3 23
4 6 42

```




```input4
4
1 2 9
2 3 8
3 4 7
4 1 5

```




```output1
1

```




```output2
2

```




```output3
39

```




```output4
0

```


