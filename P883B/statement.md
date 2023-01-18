## Description

<div><p>There are <span class="tex-span"><i>n</i></span> military men in the Berland army. Some of them have given orders to other military men by now. Given <span class="tex-span"><i>m</i></span> pairs (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>), meaning that the military man <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> gave the <span class="tex-span"><i>i</i></span>-th order to another military man <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is time for reform! The Berland Ministry of Defence plans to introduce ranks in the Berland army. Each military man should be assigned a rank — integer number between <span class="tex-span">1</span> and <span class="tex-span"><i>k</i></span>, inclusive. Some of them have been already assigned a rank, but the rest of them should get a rank soon.</p><p>Help the ministry to assign ranks to the rest of the army so that:</p><ul> <li> for each of <span class="tex-span"><i>m</i></span> orders it is true that the rank of a person giving the order (military man <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>) is strictly greater than the rank of a person receiving the order (military man <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>); </li><li> for each rank from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span> there is at least one military man with this rank. </li></ul></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of military men in the Berland army, number of orders and number of ranks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span> (in this case <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>) means that the <span class="tex-span"><i>i</i></span>-th military man has been already assigned the rank <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 0</span> means the <span class="tex-span"><i>i</i></span>-th military man doesn't have a rank yet.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain orders one per line. Each order is described with a line containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>). This line means that the <span class="tex-span"><i>i</i></span>-th order was given by the military man <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to the military man <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. For each pair <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of military men there could be several orders from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number is the rank of the <span class="tex-span"><i>i</i></span>-th military man. If there are many solutions, print any of them.</p><p>If there is no solution, print the only number <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of military men in the Berland army, number of orders and number of ranks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span> (in this case <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>) means that the <span class="tex-span"><i>i</i></span>-th military man has been already assigned the rank <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 0</span> means the <span class="tex-span"><i>i</i></span>-th military man doesn't have a rank yet.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain orders one per line. Each order is described with a line containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>). This line means that the <span class="tex-span"><i>i</i></span>-th order was given by the military man <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to the military man <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. For each pair <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of military men there could be several orders from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number is the rank of the <span class="tex-span"><i>i</i></span>-th military man. If there are many solutions, print any of them.</p><p>If there is no solution, print the only number <span class="tex-font-style-tt">-1</span>.</p>





```input1
5 3 3
0 3 0 0 2
2 4
3 4
3 5

```




```input2
7 6 5
0 4 5 4 1 0 0
6 1
3 6
3 1
7 5
7 1
7 4

```




```input3
2 2 2
2 1
1 2
2 1

```




```output1
1 3 3 2 2 

```




```output2
2 4 5 4 1 3 5 

```




```output3
-1

```


