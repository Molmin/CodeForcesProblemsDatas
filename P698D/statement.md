## Description

<div><p>Bearland is a dangerous place. Limak can’t travel on foot. Instead, he has <span class="tex-span"><i>k</i></span> magic teleportation stones. Each stone can be used <span class="tex-font-style-bf">at most once</span>. The <span class="tex-span"><i>i</i></span>-th stone allows to teleport to a point <span class="tex-span">(<i>ax</i><sub class="lower-index"><i>i</i></sub>, <i>ay</i><sub class="lower-index"><i>i</i></sub>)</span>. Limak can use stones <span class="tex-font-style-bf">in any order</span>.</p><p>There are <span class="tex-span"><i>n</i></span> monsters in Bearland. The <span class="tex-span"><i>i</i></span>-th of them stands at <span class="tex-span">(<i>mx</i><sub class="lower-index"><i>i</i></sub>, <i>my</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>The given <span class="tex-span"><i>k</i> + <i>n</i></span> points are pairwise distinct.</p><p>After each teleportation, Limak can shoot an arrow in some direction. An arrow will hit the first monster in the chosen direction. Then, both an arrow and a monster disappear. It’s dangerous to stay in one place for long, so Limak can shoot only one arrow from one place.</p><p>A monster should be afraid if it’s possible that Limak will hit it. How many monsters should be afraid of Limak?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 7</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of stones and the number of monsters.</p><p>The <span class="tex-span"><i>i</i></span>-th of following <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>ax</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>ay</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>ax</i><sub class="lower-index"><i>i</i></sub>, <i>ay</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates to which Limak can teleport using the <span class="tex-span"><i>i</i></span>-th stone.</p><p>The <span class="tex-span"><i>i</i></span>-th of last <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>mx</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>my</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>mx</i><sub class="lower-index"><i>i</i></sub>, <i>my</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the <span class="tex-span"><i>i</i></span>-th monster.</p><p>The given <span class="tex-span"><i>k</i> + <i>n</i></span> points are pairwise distinct.</p></div><div class="output-specification"><p>Print the number of monsters which should be afraid of Limak.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 7</span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of stones and the number of monsters.</p><p>The <span class="tex-span"><i>i</i></span>-th of following <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>ax</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>ay</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>ax</i><sub class="lower-index"><i>i</i></sub>, <i>ay</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates to which Limak can teleport using the <span class="tex-span"><i>i</i></span>-th stone.</p><p>The <span class="tex-span"><i>i</i></span>-th of last <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>mx</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>my</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>mx</i><sub class="lower-index"><i>i</i></sub>, <i>my</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the <span class="tex-span"><i>i</i></span>-th monster.</p><p>The given <span class="tex-span"><i>k</i> + <i>n</i></span> points are pairwise distinct.</p>

## Output

<p>Print the number of monsters which should be afraid of Limak.</p>





```input1
2 4
-2 -1
4 5
4 2
2 1
4 -1
1 -1

```




```input2
3 8
10 20
0 0
20 40
300 600
30 60
170 340
50 100
28 56
90 180
-4 -8
-1 -2

```




```output1
3

```




```output2
5

```



## Note

<p>In the first sample, there are two stones and four monsters. Stones allow to teleport to points <span class="tex-span">( - 2,  - 1)</span> and <span class="tex-span">(4, 5)</span>, marked blue in the drawing below. Monsters are at <span class="tex-span">(4, 2)</span>, <span class="tex-span">(2, 1)</span>, <span class="tex-span">(4,  - 1)</span> and <span class="tex-span">(1,  - 1)</span>, marked red. A monster at <span class="tex-span">(4,  - 1)</span> shouldn't be afraid because it's impossible that Limak will hit it with an arrow. Other three monsters can be hit and thus the answer is <span class="tex-span">3</span>.</p><center> <img class="tex-graphics" src="file://lBpdvuVi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample, five monsters should be afraid. Safe monsters are those at <span class="tex-span">(300, 600)</span>, <span class="tex-span">(170, 340)</span> and <span class="tex-span">(90, 180)</span>.</p>
