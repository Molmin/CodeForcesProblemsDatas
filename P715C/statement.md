## Description

<div><p>ZS the Coder has a large tree. It can be represented as an undirected connected graph of <span class="tex-span"><i>n</i></span> vertices numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span> and <span class="tex-span"><i>n</i> - 1</span> edges between them. There is a single <span class="tex-font-style-bf">nonzero</span> digit written on each edge.</p><p>One day, ZS the Coder was bored and decided to investigate some properties of the tree. He chose a positive integer <span class="tex-span"><i>M</i></span>, which is <span class="tex-font-style-bf">coprime</span> to <span class="tex-span">10</span>, i.e. <img align="middle" class="tex-formula" src="file://n22fzVtK.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>ZS consider an <span class="tex-font-style-bf">ordered pair</span> of distinct vertices <span class="tex-span">(<i>u</i>, <i>v</i>)</span> <span class="tex-font-style-it">interesting</span> when if he would follow the shortest path from vertex <span class="tex-span"><i>u</i></span> to vertex <span class="tex-span"><i>v</i></span> and write down all the digits he encounters on his path in the same order, he will get a decimal representaion of an integer divisible by <span class="tex-span"><i>M</i></span>.</p><p>Formally, ZS consider an ordered pair of distinct vertices <span class="tex-span">(<i>u</i>, <i>v</i>)</span> interesting if the following states true:</p><ul> <li> Let <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = <i>u</i>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub> = <i>v</i></span> be the sequence of vertices on the shortest path from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> in the order of encountering them; </li><li> Let <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>) be the digit written on the edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>; </li><li> The integer <img align="middle" class="tex-formula" src="file://VlEIO0dR.png" style="max-width: 100.0%;max-height: 100.0%;"> is divisible by <span class="tex-span"><i>M</i></span>. </li></ul><p>Help ZS the Coder find the number of interesting pairs!</p></div><div class="input-specification"><p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>,<span class="tex-span"> 1 ≤ <i>M</i> ≤ 10<sup class="upper-index">9</sup></span>, <img align="middle" class="tex-formula" src="file://HBVezqiX.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of vertices and the number ZS has chosen respectively.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain three integers each. <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, denoting an edge between vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> with digit <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> written on it (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i>,  1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of interesting (by ZS the Coder's consideration) pairs.</p></div>

## Input

<p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>,<span class="tex-span"> 1 ≤ <i>M</i> ≤ 10<sup class="upper-index">9</sup></span>, <img align="middle" class="tex-formula" src="file://HBVezqiX.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of vertices and the number ZS has chosen respectively.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain three integers each. <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, denoting an edge between vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> with digit <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> written on it (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i>,  1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>).</p>

## Output

<p>Print a single integer&nbsp;— the number of interesting (by ZS the Coder's consideration) pairs.</p>





```input1
6 7
0 1 2
4 2 4
2 0 1
3 0 9
2 5 7

```




```input2
5 11
1 2 3
2 0 3
3 0 3
4 3 3

```




```output1
7

```




```output2
8

```



## Note

<p>In the first sample case, the interesting pairs are <span class="tex-span">(0, 4), (1, 2), (1, 5), (3, 2), (2, 5), (5, 2), (3, 5)</span>. The numbers that are formed by these pairs are <span class="tex-span">14, 21, 217, 91, 7, 7, 917</span> respectively, which are all multiples of <span class="tex-span">7</span>. Note that <span class="tex-span">(2, 5)</span> and <span class="tex-span">(5, 2)</span> are considered different. </p><center> <img class="tex-graphics" src="file://BLSaQ8ks.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample case, the interesting pairs are <span class="tex-span">(4, 0), (0, 4), (3, 2), (2, 3), (0, 1), (1, 0), (4, 1), (1, 4)</span>, and <span class="tex-span">6</span> of these pairs give the number <span class="tex-span">33</span> while <span class="tex-span">2</span> of them give the number <span class="tex-span">3333</span>, which are all multiples of <span class="tex-span">11</span>.</p><center> <img class="tex-graphics" src="file://Vs0aHg4l.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
