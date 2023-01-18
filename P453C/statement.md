## Description

<div><p>Twilight Sparkle learnt that the evil Nightmare Moon would return during the upcoming Summer Sun Celebration after one thousand years of imprisonment on the moon. She tried to warn her mentor Princess Celestia, but the princess ignored her and sent her to Ponyville to check on the preparations for the celebration.</p><center> <img class="tex-graphics" src="file://raupfKJT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Twilight Sparkle wanted to track the path of Nightmare Moon. Unfortunately, she didn't know the exact path. What she knew is the parity of the number of times that each place Nightmare Moon visited. Can you help Twilight Sparkle to restore any path that is consistent with this information?</p><p>Ponyville can be represented as an undirected graph (vertices are places, edges are roads between places) without self-loops and multi-edges. The path can start and end at any place (also it can be empty). Each place can be visited multiple times. The path must not visit more than <span class="tex-span">4<i>n</i></span> places.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of places and the number of roads in Ponyville. Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), these integers describe a road between places <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span> — the parity of the number of times that each place must be visited. If <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the <span class="tex-span"><i>i</i></span>-th place must be visited even number of times, else it must be visited odd number of times.</p></div><div class="output-specification"><p>Output the number of visited places <span class="tex-span"><i>k</i></span> in the first line (<span class="tex-span">0 ≤ <i>k</i> ≤ 4<i>n</i></span>). Then output <span class="tex-span"><i>k</i></span> integers — the numbers of places in the order of path. If <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the <span class="tex-span"><i>i</i></span>-th place must appear in the path even number of times, else <span class="tex-span"><i>i</i></span>-th place must appear in the path odd number of times. Note, that given road system has no self-loops, therefore any two neighbouring places in the path must be distinct.</p><p>If there is no required path, output <span class="tex-font-style-tt">-1</span>. If there multiple possible paths, you can output any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of places and the number of roads in Ponyville. Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), these integers describe a road between places <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span> — the parity of the number of times that each place must be visited. If <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the <span class="tex-span"><i>i</i></span>-th place must be visited even number of times, else it must be visited odd number of times.</p>

## Output

<p>Output the number of visited places <span class="tex-span"><i>k</i></span> in the first line (<span class="tex-span">0 ≤ <i>k</i> ≤ 4<i>n</i></span>). Then output <span class="tex-span"><i>k</i></span> integers — the numbers of places in the order of path. If <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the <span class="tex-span"><i>i</i></span>-th place must appear in the path even number of times, else <span class="tex-span"><i>i</i></span>-th place must appear in the path odd number of times. Note, that given road system has no self-loops, therefore any two neighbouring places in the path must be distinct.</p><p>If there is no required path, output <span class="tex-font-style-tt">-1</span>. If there multiple possible paths, you can output any of them.</p>





```input1
3 2
1 2
2 3
1 1 1

```




```input2
5 7
1 2
1 3
1 4
1 5
3 4
3 5
4 5
0 1 0 1 0

```




```input3
2 0
0 0

```




```output1
3
1 2 3

```




```output2
10
2 1 3 4 5 4 5 4 3 1
```




```output3
0

```


