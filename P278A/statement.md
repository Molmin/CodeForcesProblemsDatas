## Description

<div><p>The circle line of the Berland subway has <span class="tex-span"><i>n</i></span> stations. We know the distances between all pairs of neighboring stations:</p><ul><li> <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span> is the distance between the <span class="tex-span">1</span>-st and the <span class="tex-span">2</span>-nd station;</li><li> <span class="tex-span"><i>d</i><sub class="lower-index">2</sub></span> is the distance between the <span class="tex-span">2</span>-nd and the <span class="tex-span">3</span>-rd station;<p>...</p></li><li> <span class="tex-span"><i>d</i><sub class="lower-index"><i>n</i> - 1</sub></span> is the distance between the <span class="tex-span"><i>n</i> - 1</span>-th and the <span class="tex-span"><i>n</i></span>-th station;</li><li> <span class="tex-span"><i>d</i><sub class="lower-index"><i>n</i></sub></span> is the distance between the <span class="tex-span"><i>n</i></span>-th and the <span class="tex-span">1</span>-st station.</li></ul><p>The trains go along the circle line in both directions. Find the shortest distance between stations with numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — the number of stations on the circle line. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the distances between pairs of neighboring stations. The third line contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>) — the numbers of stations, between which you need to find the shortest distance. These numbers can be the same.</p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print a single number — the length of the shortest path between stations number <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — the number of stations on the circle line. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the distances between pairs of neighboring stations. The third line contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>) — the numbers of stations, between which you need to find the shortest distance. These numbers can be the same.</p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>Print a single number — the length of the shortest path between stations number <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>.</p>





```input1
4
2 3 4 9
1 3

```




```input2
4
5 8 2 100
4 1

```




```input3
3
1 1 1
3 1

```




```input4
3
31 41 59
1 1

```




```output1
5

```




```output2
15

```




```output3
1

```




```output4
0

```



## Note

<p>In the first sample the length of path <span class="tex-span">1 → 2 → 3</span> equals 5, the length of path <span class="tex-span">1 → 4 → 3</span> equals 13.</p><p>In the second sample the length of path <span class="tex-span">4 → 1</span> is 100, the length of path <span class="tex-span">4 → 3 → 2 → 1</span> is 15.</p><p>In the third sample the length of path <span class="tex-span">3 → 1</span> is 1, the length of path <span class="tex-span">3 → 2 → 1</span> is 2.</p><p>In the fourth sample the numbers of stations are the same, so the shortest distance equals 0.</p>
