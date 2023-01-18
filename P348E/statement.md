## Description

<div><p>A long time ago there was a land called Dudeland. Dudeland consisted of <span class="tex-span"><i>n</i></span> towns connected with <span class="tex-span"><i>n</i> - 1</span> bidirectonal roads. The towns are indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and one can reach any city from any other city if he moves along the roads of the country. There are <span class="tex-span"><i>m</i></span> monasteries in Dudeland located in <span class="tex-span"><i>m</i></span> different towns. In each monastery lives a pilgrim.</p><p>At the beginning of the year, each pilgrim writes down which monastery is the farthest from the monastery he is living in. If there is more than one farthest monastery, he lists all of them. On the Big Lebowski day each pilgrim picks one town from his paper at random and starts walking to that town. </p><p>Walter hates pilgrims and wants to make as many of them unhappy as possible by preventing them from finishing their journey. He plans to destroy exactly one town that does not contain a monastery. A pilgrim becomes unhappy if all monasteries in his list become unreachable from the monastery he is living in. </p><p>You need to find the maximum number of pilgrims Walter can make unhappy. Also find the number of ways he can make this maximal number of pilgrims unhappy: the number of possible towns he can destroy.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> &lt; <i>n</i></span>). The next line contains <span class="tex-span"><i>m</i></span> distinct integers representing indices of towns that contain monasteries.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain three integers each, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, indicating that there is an edge between towns <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> of length <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>).</p></div><div class="output-specification"><p>Output two integers: the maximum number of pilgrims Walter can make unhappy and the number of ways in which he can make his plan come true.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> &lt; <i>n</i></span>). The next line contains <span class="tex-span"><i>m</i></span> distinct integers representing indices of towns that contain monasteries.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain three integers each, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, indicating that there is an edge between towns <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> of length <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>).</p>

## Output

<p>Output two integers: the maximum number of pilgrims Walter can make unhappy and the number of ways in which he can make his plan come true.</p>





```input1
8 5
7 2 5 4 8
1 2 1
2 3 2
1 4 1
4 5 2
1 6 1
6 7 8
6 8 10

```




```output1
5 1

```


