## Description

<div><p>A couple of friends, Axel and Marston are travelling across the country of Bitland. There are <span class="tex-span"><i>n</i></span> towns in Bitland, with some pairs of towns connected by one-directional roads. Each road in Bitland is either a pedestrian road or a bike road. There can be multiple roads between any pair of towns, and may even be a road from a town to itself. However, no pair of roads shares the starting and the destination towns along with their types simultaneously.</p><p>The friends are now located in the town 1 and are planning the travel route. Axel enjoys walking, while Marston prefers biking. In order to choose a route diverse and equally interesting for both friends, they have agreed upon the following procedure for choosing the road types during the travel:</p><ul><li> The route starts with a pedestrian route.</li><li> Suppose that a beginning of the route is written in a string <span class="tex-span"><i>s</i></span> of letters P (pedestrain road) and B (biking road). Then, the string <img align="middle" class="tex-formula" src="file://9Mtp1VrP.png" style="max-width: 100.0%;max-height: 100.0%;"> is appended to <span class="tex-span"><i>s</i></span>, where <img align="middle" class="tex-formula" src="file://OyKgmpKU.png" style="max-width: 100.0%;max-height: 100.0%;"> stands for the string <span class="tex-span"><i>s</i></span> with each character changed to opposite (that is, all pedestrian roads changed to bike roads, and vice versa).</li></ul><p>In the first few steps the route will look as follows: P, PB, PBBP, PBBPBPPB, PBBPBPPBBPPBPBBP, and so on.</p><p>After that the friends start travelling from the town 1 via Bitlandian roads, choosing the next road according to the next character of their route type each time. If it is impossible to choose the next road, the friends terminate their travel and fly home instead.</p><p>Help the friends to find the longest possible route that can be travelled along roads of Bitland according to the road types choosing procedure described above. If there is such a route with more than <span class="tex-span">10<sup class="upper-index">18</sup></span> roads in it, print -1 instead.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2<i>n</i><sup class="upper-index">2</sup></span>)&nbsp;— the number of towns and roads in Bitland respectively.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the roads. <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> denote start and destination towns indices of the <span class="tex-span"><i>i</i></span>-th road, and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> decribes the type of <span class="tex-span"><i>i</i></span>-th road (0 for a pedestrian road, 1 for a bike road). It is guaranteed that for each pair of distinct indices <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> such that <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>m</i></span>, either <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub></span>, or <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>j</i></sub></span>, or <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>j</i></sub></span> holds.</p></div><div class="output-specification"><p>If it is possible to find a route with length strictly greater than <span class="tex-span">10<sup class="upper-index">18</sup></span>, print -1. Otherwise, print the maximum length of a suitable path.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2<i>n</i><sup class="upper-index">2</sup></span>)&nbsp;— the number of towns and roads in Bitland respectively.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the roads. <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> denote start and destination towns indices of the <span class="tex-span"><i>i</i></span>-th road, and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> decribes the type of <span class="tex-span"><i>i</i></span>-th road (0 for a pedestrian road, 1 for a bike road). It is guaranteed that for each pair of distinct indices <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> such that <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>m</i></span>, either <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub></span>, or <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>j</i></sub></span>, or <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>j</i></sub></span> holds.</p>

## Output

<p>If it is possible to find a route with length strictly greater than <span class="tex-span">10<sup class="upper-index">18</sup></span>, print -1. Otherwise, print the maximum length of a suitable path.</p>





```input1
2 2
1 2 0
2 2 1

```




```input2
2 3
1 2 0
2 2 1
2 2 0

```




```output1
3

```




```output2
-1

```



## Note

<p>In the first sample we can obtain a route of length 3 by travelling along the road 1 from town 1 to town 2, and then following the road 2 twice from town 2 to itself.</p><p>In the second sample we can obtain an arbitrarily long route by travelling the road 1 first, and then choosing road 2 or 3 depending on the necessary type.</p>
