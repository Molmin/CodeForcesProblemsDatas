## Description

<div><p>Berland has <span class="tex-span"><i>n</i></span> cities connected by <span class="tex-span"><i>m</i></span> bidirectional roads. No road connects a city to itself, and each pair of cities is connected by no more than one road. It is <span class="tex-font-style-bf">not guaranteed</span> that you can get from any city to any other one, using only the existing roads.</p><p>The President of Berland decided to make changes to the road system and instructed the Ministry of Transport to make this reform. Now, each road should be unidirectional (only lead from one city to another).</p><p>In order not to cause great resentment among residents, the reform needs to be conducted so that there can be as few separate cities as possible. A city is considered <span class="tex-font-style-it">separate</span>, if no road leads into it, while it is allowed to have roads leading from this city.</p><p>Help the Ministry of Transport to find the minimum possible number of separate cities after the reform.</p></div><div class="input-specification"><p>The first line of the input contains two positive integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of the cities and the number of roads in Berland (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>). </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the roads: the <span class="tex-span"><i>i</i></span>-th road is determined by two distinct integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the cities connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>It is guaranteed that there is no more than one road between each pair of cities, but it is not guaranteed that from any city you can get to any other one, using only roads.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of separated cities after the reform.</p></div>

## Input

<p>The first line of the input contains two positive integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of the cities and the number of roads in Berland (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>). </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the roads: the <span class="tex-span"><i>i</i></span>-th road is determined by two distinct integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the cities connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>It is guaranteed that there is no more than one road between each pair of cities, but it is not guaranteed that from any city you can get to any other one, using only roads.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of separated cities after the reform.</p>





```input1
4 3
2 1
1 3
4 3

```




```input2
5 5
2 1
1 3
2 3
2 5
4 3

```




```input3
6 5
1 2
2 3
4 5
4 6
5 6

```




```output1
1

```




```output2
0

```




```output3
1

```



## Note

<p>In the first sample the following road orientation is allowed: <img align="middle" class="tex-formula" src="file://TBdViYNj.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://aRYEpOpY.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://LAQJZZG0.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The second sample: <img align="middle" class="tex-formula" src="file://PEpaRiwy.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://3hSXleRP.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://JRhRRBtn.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://8CACLXJN.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://bwn04oqn.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The third sample: <img align="middle" class="tex-formula" src="file://eV3O0190.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://qCfDZoDR.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://WEM7gRia.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://6MZNeP1T.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://y1iBzNGV.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
