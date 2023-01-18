## Description

<div><p>Ralph is in the Binary Country. The Binary Country consists of <span class="tex-span"><i>n</i></span> cities and <span class="tex-span">(<i>n</i> - 1)</span> bidirectional roads connecting the cities. The roads are numbered from <span class="tex-span">1</span> to <span class="tex-span">(<i>n</i> - 1)</span>, the <span class="tex-span"><i>i</i></span>-th road connects the city labeled <img align="middle" class="tex-formula" src="file://HddjTAoB.png" style="max-width: 100.0%;max-height: 100.0%;"> (here <span class="tex-span">⌊ <i>x</i>⌋</span> denotes the <span class="tex-span"><i>x</i></span> rounded down to the nearest integer) and the city labeled <span class="tex-span">(<i>i</i> + 1)</span>, and the length of the <span class="tex-span"><i>i</i></span>-th road is <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Now Ralph gives you <span class="tex-span"><i>m</i></span> queries. In each query he tells you some city <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and an integer <span class="tex-span"><i>H</i><sub class="lower-index"><i>i</i></sub></span>. He wants to make some tours starting from this city. He can choose any city in the Binary Country (including <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span>) as the terminal city for a tour. He gains happiness <span class="tex-span">(<i>H</i><sub class="lower-index"><i>i</i></sub> - <i>L</i>)</span> during a tour, where <span class="tex-span"><i>L</i></span> is the distance between the city <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and the terminal city.</p><p>Ralph is interested in tours from <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> in which he can gain positive happiness. For each query, compute the sum of happiness gains for all such tours.</p><p>Ralph will never take the same tour twice or more (in one query), he will never pass the same city twice or more in one tour.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p><span class="tex-span">(<i>n</i> - 1)</span> lines follow, each line contains one integer <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>L</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), which denotes the length of the <span class="tex-span"><i>i</i></span>-th road.</p><p><span class="tex-span"><i>m</i></span> lines follow, each line contains two integers <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>H</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>A</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>H</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, on the <span class="tex-span"><i>i</i></span>-th line print one integer&nbsp;— the answer for the <span class="tex-span"><i>i</i></span>-th query.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p><span class="tex-span">(<i>n</i> - 1)</span> lines follow, each line contains one integer <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>L</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), which denotes the length of the <span class="tex-span"><i>i</i></span>-th road.</p><p><span class="tex-span"><i>m</i></span> lines follow, each line contains two integers <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>H</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>A</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>H</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, on the <span class="tex-span"><i>i</i></span>-th line print one integer&nbsp;— the answer for the <span class="tex-span"><i>i</i></span>-th query.</p>





```input1
2 2
5
1 8
2 4

```




```input2
6 4
2
1
1
3
2
2 4
1 3
3 2
1 7

```




```output1
11
4

```




```output2
11
6
3
28

```



## Note

<p>Here is the explanation for the second sample.</p><p>Ralph's first query is to start tours from city <span class="tex-span">2</span> and <span class="tex-span"><i>H</i><sub class="lower-index"><i>i</i></sub></span> equals to <span class="tex-span">4</span>. Here are the options:</p><ul> <li> He can choose city <span class="tex-span">5</span> as his terminal city. Since the distance between city <span class="tex-span">5</span> and city <span class="tex-span">2</span> is <span class="tex-span">3</span>, he can gain happiness <span class="tex-span">4 - 3 = 1</span>. </li><li> He can choose city <span class="tex-span">4</span> as his terminal city and gain happiness <span class="tex-span">3</span>. </li><li> He can choose city <span class="tex-span">1</span> as his terminal city and gain happiness <span class="tex-span">2</span>. </li><li> He can choose city <span class="tex-span">3</span> as his terminal city and gain happiness <span class="tex-span">1</span>. </li><li> Note that Ralph can choose city <span class="tex-span">2</span> as his terminal city and gain happiness <span class="tex-span">4</span>. </li><li> Ralph won't choose city <span class="tex-span">6</span> as his terminal city because the distance between city <span class="tex-span">6</span> and city <span class="tex-span">2</span> is <span class="tex-span">5</span>, which leads to negative happiness for Ralph. </li></ul><p>So the answer for the first query is <span class="tex-span">1 + 3 + 2 + 1 + 4 = 11</span>.</p>
