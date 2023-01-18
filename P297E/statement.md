## Description

<div><p>The polar bears have discovered a gigantic circular piece of floating ice with some mystic carvings on it. There are <span class="tex-span"><i>n</i></span> lines carved on the ice. Each line connects two points on the boundary of the ice (we call these points <span class="tex-font-style-it">endpoints</span>). The endpoints are numbered <span class="tex-span">1, 2, ..., 2<i>n</i></span> counter-clockwise along the circumference. No two lines share an endpoint.</p><p>Now a group of 6 polar bears (Alice, Bob, Carol, Dave, Eve, Frank) are going to build caves on the endpoints. Each polar bear would build a cave and live in it. No two polar bears can build a cave on the same endpoints. Alice and Bob is a pair of superstitious lovers. They believe the lines are carved by aliens (or humans, which are pretty much the same thing to polar bears), and have certain spiritual power. Therefore they want to build their caves on two endpoints which are connected by a line. The same for Carol and Dave, Eve and Frank.</p><p>The <span class="tex-font-style-it">distance</span> between two caves X and Y is defined as one plus minimum number of other caves one need to pass through in order to travel from X to Y along the boundary of the ice (endpoints without caves are not counted).</p><p>To ensure fairness, the distances between the three pairs of lovers have to be the same (that is, the distance between Alice and Bob, the distance between Carol and Dave, and the distance between Eve and Frank are the same).</p><p>The figures below show two different configurations, where the dots on the circle are the endpoints. The configuration on the left is not valid. Although each pair of lovers (A and B, C and D, E and F) is connected a line, the distance requirement is not satisfied. The distance between A and B is 2 (one can go from A to B in the clockwise direction passing through F). The distance between E and F is also 2. However, the distance between C and D is 1 (one can go from C to D in the counter-clockwise direction without passing through any other caves). The configuration on the right is valid. All three pairs have the same distance 1.</p><center> <img class="tex-graphics" src="file://kA2NZmUx.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Count the number of ways to build the caves under the requirements. Two configurations are considered the same if the same set of 6 endpoints are used.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span>(<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of lines.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>n</i></span>), which means that there is a line carved on the ice connecting the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>–th and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>–th endpoint. </p><p>It's guaranteed that each endpoints touches exactly one line.</p></div><div class="output-specification"><p>Print the number of ways to build the caves.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span>(<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of lines.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>n</i></span>), which means that there is a line carved on the ice connecting the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>–th and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>–th endpoint. </p><p>It's guaranteed that each endpoints touches exactly one line.</p>

## Output

<p>Print the number of ways to build the caves.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4
5 4
1 2
6 7
8 3

```




```input2
8
1 7
2 4
3 9
5 11
6 8
10 16
13 15
14 12

```




```output1
2

```




```output2
6

```



## Note

<p>The second sample corresponds to the figure in the problem statement.</p>
