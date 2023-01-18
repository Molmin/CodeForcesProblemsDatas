## Description

<div><p>There are <span class="tex-span"><i>n</i></span> stone quarries in Petrograd.</p><p>Each quarry owns <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> dumpers (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). It is known that the first dumper of the <span class="tex-span"><i>i</i></span>-th quarry has <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> stones in it, the second dumper has <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + 1</span> stones in it, the third has <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + 2</span>, and the <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>-th dumper (the last for the <span class="tex-span"><i>i</i></span>-th quarry) has <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + <i>m</i><sub class="lower-index"><i>i</i></sub> - 1</span> stones in it.</p><p>Two oligarchs play a well-known game Nim. Players take turns removing stones from dumpers. On each turn, a player can select any dumper and remove any non-zero amount of stones from it. The player who cannot take a stone loses.</p><p>Your task is to find out which oligarch will win, provided that both of them play optimally. The oligarchs asked you not to reveal their names. So, let's call the one who takes the first stone «<span class="tex-font-style-tt">tolik</span>» and the other one «<span class="tex-font-style-tt">bolik</span>».</p></div><div class="input-specification"><p>The first line of the input contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the amount of quarries. Then there follow <span class="tex-span"><i>n</i></span> lines, each of them contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">16</sup></span>) — the amount of stones in the first dumper of the <span class="tex-span"><i>i</i></span>-th quarry and the number of dumpers at the <span class="tex-span"><i>i</i></span>-th quarry.</p></div><div class="output-specification"><p>Output «<span class="tex-font-style-tt">tolik</span>» if the oligarch who takes a stone first wins, and «<span class="tex-font-style-tt">bolik</span>» otherwise.</p></div>

## Input

<p>The first line of the input contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the amount of quarries. Then there follow <span class="tex-span"><i>n</i></span> lines, each of them contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">16</sup></span>) — the amount of stones in the first dumper of the <span class="tex-span"><i>i</i></span>-th quarry and the number of dumpers at the <span class="tex-span"><i>i</i></span>-th quarry.</p>

## Output

<p>Output «<span class="tex-font-style-tt">tolik</span>» if the oligarch who takes a stone first wins, and «<span class="tex-font-style-tt">bolik</span>» otherwise.</p>





```input1
2
2 1
3 2

```




```input2
4
1 1
1 1
1 1
1 1

```




```output1
tolik

```




```output2
bolik

```


