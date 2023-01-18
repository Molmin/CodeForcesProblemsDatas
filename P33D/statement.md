## Description

<div><p>Berland is facing dark times again. The army of evil lord Van de Mart is going to conquer the whole kingdom. To the council of war called by the Berland's king Valery the Severe came <span class="tex-span"><i>n</i></span> knights. After long discussions it became clear that the kingdom has exactly <span class="tex-span"><i>n</i></span> control points (if the enemy conquers at least one of these points, the war is lost) and each knight will occupy one of these points. </p><p>Berland is divided into <span class="tex-span"><i>m</i> + 1</span> regions with <span class="tex-span"><i>m</i></span> fences, and the only way to get from one region to another is to climb over the fence. Each fence is a circle on a plane, no two fences have common points, and no control point is on the fence. You are given <span class="tex-span"><i>k</i></span> pairs of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. For each pair you have to find out: how many fences a knight from control point with index <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> has to climb over to reach control point <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (in case when Van de Mart attacks control point <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> first). As each knight rides a horse (it is very difficult to throw a horse over a fence), you are to find out for each pair the minimum amount of fences to climb over.</p></div><div class="input-specification"><p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 100000</span>). Then follow <span class="tex-span"><i>n</i></span> lines, each containing two integers <span class="tex-span"><i>Kx</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>Ky</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>Kx</i><sub class="lower-index"><i>i</i></sub>, <i>Ky</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — coordinates of control point with index <span class="tex-span"><i>i</i></span>. Control points can coincide.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines describes fence with index <span class="tex-span"><i>i</i></span> with three integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>Cx</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>Cy</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>Cx</i><sub class="lower-index"><i>i</i></sub>, <i>Cy</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — radius and center of the circle where the corresponding fence is situated.</p><p>Then follow <span class="tex-span"><i>k</i></span> pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), each in a separate line — requests that you have to answer. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> can coincide.</p></div><div class="output-specification"><p>Output exactly <span class="tex-span"><i>k</i></span> lines, each containing one integer — the answer to the corresponding request.</p></div>

## Input

<p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 100000</span>). Then follow <span class="tex-span"><i>n</i></span> lines, each containing two integers <span class="tex-span"><i>Kx</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>Ky</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>Kx</i><sub class="lower-index"><i>i</i></sub>, <i>Ky</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — coordinates of control point with index <span class="tex-span"><i>i</i></span>. Control points can coincide.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines describes fence with index <span class="tex-span"><i>i</i></span> with three integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>Cx</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>Cy</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>Cx</i><sub class="lower-index"><i>i</i></sub>, <i>Cy</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — radius and center of the circle where the corresponding fence is situated.</p><p>Then follow <span class="tex-span"><i>k</i></span> pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), each in a separate line — requests that you have to answer. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> can coincide.</p>

## Output

<p>Output exactly <span class="tex-span"><i>k</i></span> lines, each containing one integer — the answer to the corresponding request.</p>





```input1
2 1 1
0 0
3 3
2 0 0
1 2

```




```input2
2 3 1
0 0
4 4
1 0 0
2 0 0
3 0 0
1 2

```




```output1
1

```




```output2
3

```


