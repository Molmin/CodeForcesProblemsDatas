## Description

<div><p>ZS the Coder and Chris the Baboon has explored Udayland for quite some time. They realize that it consists of <span class="tex-span"><i>n</i></span> towns numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p><p>There are <span class="tex-span"><i>n</i></span> directed roads in the Udayland. <span class="tex-span"><i>i</i></span>-th of them goes from town <span class="tex-span"><i>i</i></span> to some other town <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>). ZS the Coder can flip the direction of any road in Udayland, i.e. if it goes from town <span class="tex-span"><i>A</i></span> to town <span class="tex-span"><i>B</i></span> before the flip, it will go from town <span class="tex-span"><i>B</i></span> to town <span class="tex-span"><i>A</i></span> after.</p><p>ZS the Coder considers the roads in the Udayland <span class="tex-font-style-it">confusing</span>, if there is a sequence of distinct towns <span class="tex-span"><i>A</i><sub class="lower-index">1</sub>, <i>A</i><sub class="lower-index">2</sub>, ..., <i>A</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span"><i>k</i> &gt; 1</span>) such that for every <span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span> there is a road from town <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> to town <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i> + 1</sub></span> and another road from town <span class="tex-span"><i>A</i><sub class="lower-index"><i>k</i></sub></span> to town <span class="tex-span"><i>A</i><sub class="lower-index">1</sub></span>. In other words, the roads are confusing if <span class="tex-font-style-bf">some of them</span> form a directed cycle of some towns.</p><p>Now ZS the Coder wonders how many sets of roads (there are <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> variants) in initial configuration can he choose to flip such that after flipping each road in the set exactly once, the resulting network will <span class="tex-font-style-bf">not</span> be confusing.</p><p>Note that it is allowed that after the flipping there are more than one directed road from some town and possibly some towns with no roads leading out of it, or multiple roads between any pair of cities.</p></div><div class="input-specification"><p>The first line of the input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of towns in Udayland.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i>)</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes a road going from town <span class="tex-span"><i>i</i></span> to town <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of ways to flip some set of the roads so that the resulting whole set of all roads is not confusing. Since this number may be too large, print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of towns in Udayland.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i>)</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes a road going from town <span class="tex-span"><i>i</i></span> to town <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print a single integer&nbsp;— the number of ways to flip some set of the roads so that the resulting whole set of all roads is not confusing. Since this number may be too large, print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
2 3 1

```




```input2
4
2 1 1 1

```




```input3
5
2 4 2 5 3

```




```output1
6

```




```output2
8

```




```output3
28

```



## Note

<p>Consider the first sample case. There are <span class="tex-span">3</span> towns and <span class="tex-span">3</span> roads. The towns are numbered from <span class="tex-span">1</span> to <span class="tex-span">3</span> and the roads are <img align="middle" class="tex-formula" src="file://v1s5fOVE.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://XHPfwjJm.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://O3g6mHaz.png" style="max-width: 100.0%;max-height: 100.0%;"> initially. Number the roads <span class="tex-span">1</span> to <span class="tex-span">3</span> in this order. </p><p>The sets of roads that ZS the Coder can flip (to make them not confusing) are <span class="tex-span">{1}, {2}, {3}, {1, 2}, {1, 3}, {2, 3}</span>. Note that the empty set is invalid because if no roads are flipped, then towns <span class="tex-span">1, 2, 3</span> is form a directed cycle, so it is confusing. Similarly, flipping all roads is confusing too. Thus, there are a total of <span class="tex-span">6</span> possible sets ZS the Coder can flip.</p><p>The sample image shows all possible ways of orienting the roads from the first sample such that the network is <span class="tex-font-style-bf">not confusing</span>.</p><p><img class="tex-graphics" src="file://W7KHqZa6.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
