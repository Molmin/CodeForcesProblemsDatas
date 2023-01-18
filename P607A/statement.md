## Description

<div><p>There are <span class="tex-span"><i>n</i></span> beacons located at distinct positions on a number line. The <span class="tex-span"><i>i</i></span>-th beacon has position <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and power level <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. When the <span class="tex-span"><i>i</i></span>-th beacon is activated, it destroys all beacons to its left (direction of decreasing coordinates) within distance <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> inclusive. The beacon itself is not destroyed however. Saitama will activate the beacons one at a time from right to left. If a beacon is destroyed, it cannot be activated.</p><p>Saitama wants Genos to add a beacon <span class="tex-font-style-bf">strictly to the right</span> of all the existing beacons, with any position and any power level, such that the least possible number of beacons are destroyed. Note that Genos's placement of the beacon means it will be the first beacon activated. Help Genos by finding the minimum number of beacons that could be destroyed.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the initial number of beacons.</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the position and power level of the <span class="tex-span"><i>i</i></span>-th beacon respectively. No two beacons will have the same position, so <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub></span> if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of beacons that could be destroyed if exactly one beacon is added.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the initial number of beacons.</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the position and power level of the <span class="tex-span"><i>i</i></span>-th beacon respectively. No two beacons will have the same position, so <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub></span> if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of beacons that could be destroyed if exactly one beacon is added.</p>





```input1
4
1 9
3 1
6 1
7 4

```




```input2
7
1 1
2 1
3 1
4 1
5 1
6 1
7 1

```




```output1
1

```




```output2
3

```



## Note

<p>For the first sample case, the minimum number of beacons destroyed is <span class="tex-span">1</span>. One way to achieve this is to place a beacon at position <span class="tex-span">9</span> with power level <span class="tex-span">2</span>.</p><p>For the second sample case, the minimum number of beacons destroyed is <span class="tex-span">3</span>. One way to achieve this is to place a beacon at position <span class="tex-span">1337</span> with power level <span class="tex-span">42</span>.</p>
