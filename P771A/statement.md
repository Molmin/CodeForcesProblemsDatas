## Description

<div><p>Bear Limak examines a social network. Its main functionality is that two members can become friends (then they can talk with each other and share funny pictures).</p><p>There are <span class="tex-span"><i>n</i></span> members, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. <span class="tex-span"><i>m</i></span> pairs of members are friends. Of course, a member can't be a friend with themselves.</p><p>Let <span class="tex-font-style-tt">A-B</span> denote that members <span class="tex-font-style-tt">A</span> and <span class="tex-font-style-tt">B</span> are friends. Limak thinks that a network is <span class="tex-font-style-it">reasonable</span> if and only if the following condition is satisfied: For every three <span class="tex-font-style-bf">distinct</span> members (<span class="tex-font-style-tt">X</span>, <span class="tex-font-style-tt">Y</span>, <span class="tex-font-style-tt">Z</span>), if <span class="tex-font-style-tt">X-Y</span> and <span class="tex-font-style-tt">Y-Z</span> then also <span class="tex-font-style-tt">X-Z</span>.</p><p>For example: if Alan and Bob are friends, and Bob and Ciri are friends, then Alan and Ciri should be friends as well.</p><p>Can you help Limak and check if the network is reasonable? Print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" accordingly, without the quotes.</p></div><div class="input-specification"><p>The first line of the input contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 150 000</span>, <img align="middle" class="tex-formula" src="file://wypwniDP.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of members and the number of pairs of members that are friends.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contains two distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). Members <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are friends with each other. No pair of members will appear more than once in the input.</p></div><div class="output-specification"><p>If the given network is reasonable, print "<span class="tex-font-style-tt">YES</span>" in a single line (without the quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" in a single line (without the quotes).</p></div>

## Input

<p>The first line of the input contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 150 000</span>, <img align="middle" class="tex-formula" src="file://wypwniDP.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of members and the number of pairs of members that are friends.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contains two distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). Members <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are friends with each other. No pair of members will appear more than once in the input.</p>

## Output

<p>If the given network is reasonable, print "<span class="tex-font-style-tt">YES</span>" in a single line (without the quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" in a single line (without the quotes).</p>





```input1
4 3
1 3
3 4
1 4

```




```input2
4 4
3 1
2 3
3 4
1 2

```




```input3
10 4
4 3
5 10
8 9
1 2

```




```input4
3 2
1 2
2 3

```




```output1
YES

```




```output2
NO

```




```output3
YES

```




```output4
NO

```



## Note

<p>The drawings below show the situation in the first sample (on the left) and in the second sample (on the right). Each edge represents two members that are friends. The answer is "<span class="tex-font-style-tt">NO</span>" in the second sample because members <span class="tex-span">(2, 3)</span> are friends and members <span class="tex-span">(3, 4)</span> are friends, while members <span class="tex-span">(2, 4)</span> are not.</p><center> <img class="tex-graphics" src="file://tR3wQPIA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
