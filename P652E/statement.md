## Description

<div><p>Johnny is playing a well-known computer game. The game are in some country, where the player can freely travel, pass quests and gain an experience.</p><p>In that country there are <span class="tex-span"><i>n</i></span> islands and <span class="tex-span"><i>m</i></span> bridges between them, so you can travel from any island to any other. In the middle of some bridges are lying ancient powerful artifacts. Johnny is not interested in artifacts, but he can get some money by selling some artifact.</p><p>At the start Johnny is in the island <span class="tex-span"><i>a</i></span> and the artifact-dealer is in the island <span class="tex-span"><i>b</i></span> (possibly they are on the same island). Johnny wants to find some artifact, come to the dealer and sell it. The only difficulty is that bridges are too old and destroying right after passing over them. Johnnie's character can't swim, fly and teleport, so the problem became too difficult.</p><p>Note that Johnny can't pass the half of the bridge, collect the artifact and return to the same island. </p><p>Determine if Johnny can find some artifact and sell it.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of islands and bridges in the game.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of the bridge — three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">0 ≤ <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the islands connected by the <span class="tex-span"><i>i</i></span>-th bridge, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> equals to one if that bridge contains an artifact and to zero otherwise. There are no more than one bridge between any pair of islands. It is guaranteed that it's possible to travel between any pair of islands.</p><p>The last line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>) — the islands where are Johnny and the artifact-dealer respectively.</p></div><div class="output-specification"><p>If Johnny can find some artifact and sell it print the only word "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise print the word "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of islands and bridges in the game.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of the bridge — three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">0 ≤ <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the islands connected by the <span class="tex-span"><i>i</i></span>-th bridge, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> equals to one if that bridge contains an artifact and to zero otherwise. There are no more than one bridge between any pair of islands. It is guaranteed that it's possible to travel between any pair of islands.</p><p>The last line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>) — the islands where are Johnny and the artifact-dealer respectively.</p>

## Output

<p>If Johnny can find some artifact and sell it print the only word "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise print the word "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
6 7
1 2 0
2 3 0
3 1 0
3 4 1
4 5 0
5 6 0
6 4 0
1 6

```




```input2
5 4
1 2 0
2 3 0
3 4 0
2 5 1
1 4

```




```input3
5 6
1 2 0
2 3 0
3 1 0
3 4 0
4 5 1
5 3 0
1 2

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


