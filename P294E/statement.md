## Description

<div><p>The great Shaass is the new king of the Drakht empire. The empire has <span class="tex-span"><i>n</i></span> cities which are connected by <span class="tex-span"><i>n</i> - 1</span> bidirectional roads. Each road has an specific length and connects a pair of cities. There's a unique simple path connecting each pair of cities.</p><p>His majesty the great Shaass has decided to tear down one of the roads and build another road with the same length between some pair of cities. He should build such road that it's still possible to travel from each city to any other city. He might build the same road again.</p><p>You as his advisor should help him to find a way to make the described action. You should find the way that minimize the total sum of pairwise distances between cities after the action. So calculate the minimum sum.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> denoting the number of cities in the empire, <span class="tex-span">(2 ≤ <i>n</i> ≤ 5000)</span>. The next <span class="tex-span"><i>n</i> - 1</span> lines each contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> showing that two cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are connected using a road of length <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>On the only line of the output print the minimum pairwise sum of distances between the cities.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> denoting the number of cities in the empire, <span class="tex-span">(2 ≤ <i>n</i> ≤ 5000)</span>. The next <span class="tex-span"><i>n</i> - 1</span> lines each contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> showing that two cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are connected using a road of length <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>On the only line of the output print the minimum pairwise sum of distances between the cities.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
3
1 2 2
1 3 4

```




```input2
6
1 2 1
2 3 1
3 4 1
4 5 1
5 6 1

```




```input3
6
1 3 1
2 3 1
3 4 100
4 5 2
4 6 1

```




```output1
12

```




```output2
29

```




```output3
825

```


