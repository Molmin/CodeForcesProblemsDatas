## Description

<div><p>Gerald plays the following game. He has a checkered field of size <span class="tex-span"><i>n</i> × <i>n</i></span> cells, where <span class="tex-span"><i>m</i></span> various cells are banned. Before the game, he has to put a few chips on some border (but not corner) board cells. Then for <span class="tex-span"><i>n</i> - 1</span> minutes, Gerald every minute moves each chip into an adjacent cell. He moves each chip from its original edge to the opposite edge. Gerald loses in this game in each of the three cases:</p><ul> <li> At least one of the chips at least once fell to the banned cell. </li><li> At least once two chips were on the same cell. </li><li> At least once two chips swapped in a minute (for example, if you stand two chips on two opposite border cells of a row with even length, this situation happens in the middle of the row). </li></ul><p>In that case he loses and earns <span class="tex-span">0</span> points. When nothing like that happened, he wins and earns the number of points equal to the number of chips he managed to put on the board. Help Gerald earn the most points.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the field and the number of banned cells. Next <span class="tex-span"><i>m</i></span> lines each contain two space-separated integers. Specifically, the <span class="tex-span"><i>i</i></span>-th of these lines contains numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th banned cell. All given cells are distinct.</p><p>Consider the field rows numbered from top to bottom from 1 to <span class="tex-span"><i>n</i></span>, and the columns — from left to right from 1 to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the maximum points Gerald can earn in this game.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the field and the number of banned cells. Next <span class="tex-span"><i>m</i></span> lines each contain two space-separated integers. Specifically, the <span class="tex-span"><i>i</i></span>-th of these lines contains numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th banned cell. All given cells are distinct.</p><p>Consider the field rows numbered from top to bottom from 1 to <span class="tex-span"><i>n</i></span>, and the columns — from left to right from 1 to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print a single integer — the maximum points Gerald can earn in this game.</p>





```input1
3 1
2 2

```




```input2
3 0

```




```input3
4 3
3 1
3 2
3 3

```




```output1
0

```




```output2
1

```




```output3
1

```



## Note

<p>In the first test the answer equals zero as we can't put chips into the corner cells.</p><p>In the second sample we can place one chip into either cell (1, 2), or cell (3, 2), or cell (2, 1), or cell (2, 3). We cannot place two chips.</p><p>In the third sample we can only place one chip into either cell (2, 1), or cell (2, 4).</p>
