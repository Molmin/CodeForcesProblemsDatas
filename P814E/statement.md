## Description

<div><p>Those unwilling to return home from a long journey, will be affected by the oddity of the snail and lose their way. Mayoi, the oddity's carrier, wouldn't like this to happen, but there's nothing to do with this before a cure is figured out. For now, she would only like to know the enormous number of possibilities to be faced with if someone gets lost.</p><p>There are <span class="tex-span"><i>n</i></span> towns in the region, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The town numbered <span class="tex-span">1</span> is called the capital. The traffic network is formed by bidirectional roads connecting pairs of towns. No two roads connect the same pair of towns, and no road connects a town with itself. The time needed to travel through each of the roads is the same. Lost travelers will not be able to find out how the towns are connected, but the residents can help them by providing the following facts: </p><ul> <li> Starting from each town other than the capital, the shortest path (i.e. the path passing through the minimum number of roads) to the capital exists, and is unique; </li><li> Let <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> be the number of roads on the shortest path from town <span class="tex-span"><i>i</i></span> to the capital, then <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≥ <i>l</i><sub class="lower-index"><i>i</i> - 1</sub></span> holds for all <span class="tex-span">2 ≤ <i>i</i> ≤ <i>n</i></span>; </li><li> For town <span class="tex-span"><i>i</i></span>, the number of roads connected to it is denoted by <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, which equals either <span class="tex-span">2</span> or <span class="tex-span">3</span>. </li></ul><p>You are to count the number of different ways in which the towns are connected, and give the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Two ways of connecting towns are considered different if a pair <span class="tex-span">(<i>u</i>, <i>v</i>)</span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) exists such there is a road between towns <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> in one of them but not in the other.</p></div><div class="input-specification"><p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50</span>) — the number of towns.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) — the number of roads connected to towns <span class="tex-span">1, 2, ..., <i>n</i></span>, respectively. It is guaranteed that the sum of <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> over all <span class="tex-span"><i>i</i></span> is even.</p></div><div class="output-specification"><p>Output one integer — the total number of different possible ways in which the towns are connected, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50</span>) — the number of towns.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) — the number of roads connected to towns <span class="tex-span">1, 2, ..., <i>n</i></span>, respectively. It is guaranteed that the sum of <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> over all <span class="tex-span"><i>i</i></span> is even.</p>

## Output

<p>Output one integer — the total number of different possible ways in which the towns are connected, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4
3 2 3 2

```




```input2
5
2 3 3 2 2

```




```input3
5
2 2 2 2 2

```




```input4
20
2 2 2 2 3 2 3 2 2 2 2 2 2 2 2 2 2 3 3 2

```




```output1
1

```




```output2
2

```




```output3
2

```




```output4
82944

```



## Note

<p>In the first example, the following structure is the only one to satisfy the constraints, the distances from towns <span class="tex-span">2, 3, 4</span> to the capital are all <span class="tex-span">1</span>.</p><center> <img class="tex-graphics" src="file://WXEM9zhC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, the following two structures satisfy the constraints.</p><center> <img class="tex-graphics" src="file://K0ObhqNB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
