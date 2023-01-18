## Description

<div><p>Slava plays his favorite game "Peace Lightning". Now he is flying a bomber on a very specific map.</p><p>Formally, map is a checkered field of size <span class="tex-span">1 × <i>n</i></span>, the cells of which are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, in each cell there can be one or several tanks. Slava doesn't know the number of tanks and their positions, because he flies very high, but he can drop a bomb in any cell. All tanks in this cell will be damaged.</p><p>If a tank takes damage for the first time, it instantly moves to one of the neighboring cells (a tank in the cell <span class="tex-span"><i>n</i></span> can only move to the cell <span class="tex-span"><i>n</i> - 1</span>, a tank in the cell <span class="tex-span">1</span> can only move to the cell <span class="tex-span">2</span>). If a tank takes damage for the second time, it's counted as destroyed and never moves again. The tanks move only when they are damaged for the first time, they do not move by themselves.</p><p>Help Slava to destroy all tanks using as few bombs as possible.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) — the size of the map.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>m</i></span> — the minimum number of bombs Slava needs to destroy all tanks.</p><p>In the second line print <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>m</i></sub></span>. The number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> means that the <span class="tex-span"><i>i</i></span>-th bomb should be dropped at the cell <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) — the size of the map.</p>

## Output

<p>In the first line print <span class="tex-span"><i>m</i></span> — the minimum number of bombs Slava needs to destroy all tanks.</p><p>In the second line print <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>m</i></sub></span>. The number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> means that the <span class="tex-span"><i>i</i></span>-th bomb should be dropped at the cell <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>If there are multiple answers, you can print any of them.</p>





```input1
2

```




```input2
3

```




```output1
3
2 1 2
```




```output2
4
2 1 3 2
```


