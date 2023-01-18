## Description

<div><p>Kirito is stuck on a level of the MMORPG he is playing now. To move on in the game, he's got to defeat all <span class="tex-span"><i>n</i></span> dragons that live on this level. Kirito and the dragons have <span class="tex-font-style-underline">strength</span>, which is represented by an integer. In the duel between two opponents the duel's outcome is determined by their strength. Initially, Kirito's strength equals <span class="tex-span"><i>s</i></span>.</p><p>If Kirito starts duelling with the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) dragon and Kirito's strength is not greater than the dragon's strength <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, then Kirito loses the duel and dies. But if Kirito's strength is greater than the dragon's strength, then he defeats the dragon and gets a bonus strength increase by <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Kirito can fight the dragons in any order. Determine whether he can move on to the next level of the game, that is, defeat all dragons without a single loss.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>). Then <span class="tex-span"><i>n</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the <span class="tex-span"><i>i</i></span>-th dragon's strength and the bonus for defeating it.</p></div><div class="output-specification"><p>On a single line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if Kirito can move on to the next level and print "<span class="tex-font-style-tt">NO</span>" (without the quotes), if he can't.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>). Then <span class="tex-span"><i>n</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the <span class="tex-span"><i>i</i></span>-th dragon's strength and the bonus for defeating it.</p>

## Output

<p>On a single line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if Kirito can move on to the next level and print "<span class="tex-font-style-tt">NO</span>" (without the quotes), if he can't.</p>





```input1
2 2
1 99
100 0

```




```input2
10 1
100 100

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample Kirito's strength initially equals 2. As the first dragon's strength is less than 2, Kirito can fight it and defeat it. After that he gets the bonus and his strength increases to <span class="tex-span">2 + 99 = 101</span>. Now he can defeat the second dragon and move on to the next level.</p><p>In the second sample Kirito's strength is too small to defeat the only dragon and win.</p>
