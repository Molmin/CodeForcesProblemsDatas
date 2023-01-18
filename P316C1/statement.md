## Description

<div><p>Smart Beaver is careful about his appearance and pays special attention to shoes so he has a huge number of pairs of shoes from the most famous brands of the forest. He's trying to handle his shoes carefully so that each pair stood side by side. But by the end of the week because of his very active lifestyle in his dressing room becomes a mess.</p><p>Smart Beaver from ABBYY is not only the brightest beaver in the area, but he also is the most domestically oriented. For example, on Mondays the Smart Beaver cleans everything in his home.</p><p>It's Monday morning. Smart Beaver does not want to spend the whole day cleaning, besides, there is much in to do and it’s the gym day, so he wants to clean up as soon as possible. Now the floors are washed, the dust is wiped off — it’s time to clean up in the dressing room. But as soon as the Smart Beaver entered the dressing room, all plans for the day were suddenly destroyed: chaos reigned there and it seemed impossible to handle, even in a week. Give our hero some hope: tell him what is the minimum number of shoes need to change the position to make the dressing room neat.</p><p>The dressing room is rectangular and is divided into <span class="tex-span"><i>n</i> × <i>m</i></span> equal squares, each square contains exactly one shoe. Each pair of shoes has a unique number that is integer from <span class="tex-span">1</span> to <img align="middle" class="tex-formula" src="file://WiNRIZM6.png" style="max-width: 100.0%;max-height: 100.0%;">, more formally, a square with coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span> contains an integer number of the pair which is lying on it. The Smart Beaver believes that the dressing room is neat only when each pair of sneakers lies together. We assume that the pair of sneakers in squares <span class="tex-span">(<i>i</i><sub class="lower-index">1</sub>, <i>j</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>i</i><sub class="lower-index">2</sub>, <i>j</i><sub class="lower-index">2</sub>)</span> lies together if <span class="tex-span">|<i>i</i><sub class="lower-index">1</sub> - <i>i</i><sub class="lower-index">2</sub>| + |<i>j</i><sub class="lower-index">1</sub> - <i>j</i><sub class="lower-index">2</sub>| = 1</span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>. They correspond to the dressing room size. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> space-separated integers each. Those numbers describe the dressing room. Each number corresponds to a snicker. </p><p>It is guaranteed that: </p><ul> <li> <span class="tex-span"><i>n</i>·<i>m</i></span> is even. </li><li> All numbers, corresponding to the numbers of pairs of shoes in the dressing room, will lie between <span class="tex-span">1</span> and <img align="middle" class="tex-formula" src="file://JFSe57fr.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> Each number from <span class="tex-span">1</span> to <img align="middle" class="tex-formula" src="file://VxPl5NEE.png" style="max-width: 100.0%;max-height: 100.0%;"> will occur exactly twice. </li></ul><p>The input limits for scoring 30 points are (subproblem C1): </p><ul> <li> <span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 8</span>. </li></ul><p>The input limits for scoring 100 points are (subproblems C1+C2): </p><ul> <li> <span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 80</span>. </li></ul></div><div class="output-specification"><p>Print exactly one integer — the minimum number of the sneakers that need to change their location.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>. They correspond to the dressing room size. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> space-separated integers each. Those numbers describe the dressing room. Each number corresponds to a snicker. </p><p>It is guaranteed that: </p><ul> <li> <span class="tex-span"><i>n</i>·<i>m</i></span> is even. </li><li> All numbers, corresponding to the numbers of pairs of shoes in the dressing room, will lie between <span class="tex-span">1</span> and <img align="middle" class="tex-formula" src="file://JFSe57fr.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> Each number from <span class="tex-span">1</span> to <img align="middle" class="tex-formula" src="file://VxPl5NEE.png" style="max-width: 100.0%;max-height: 100.0%;"> will occur exactly twice. </li></ul><p>The input limits for scoring 30 points are (subproblem C1): </p><ul> <li> <span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 8</span>. </li></ul><p>The input limits for scoring 100 points are (subproblems C1+C2): </p><ul> <li> <span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 80</span>. </li></ul>

## Output

<p>Print exactly one integer — the minimum number of the sneakers that need to change their location.</p>





```input1
2 3
1 1 2
2 3 3

```




```input2
3 4
1 3 2 6
2 1 5 6
4 4 5 3

```




```output1
2

```




```output2
4

```



## Note

<center> <img class="tex-graphics" src="file://HpCIbgoI.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> The second sample. </span> </center>
