## Description

<div><p>Igor K. very much likes a multiplayer role playing game WineAge II. Who knows, perhaps, that might be the reason for his poor performance at the university. As any person who plays the game, he is interested in equipping his hero with as good weapon and outfit as possible. </p><p>One day, as he was reading the game's forum yet again, he discovered a very interesting fact. As it turns out, each weapon in the game is characterised with <span class="tex-span"><i>k</i></span> different numbers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>. They are called hit indicators and according to the game developers' plan they are pairwise coprime. </p><p>The damage that is inflicted during a hit depends not only on the weapon's characteristics, but also on the hero's strength parameter. Thus, if the hero's strength equals <span class="tex-span"><i>n</i></span>, than the inflicted damage will be calculated as the number of numbers on the segment <img align="middle" class="tex-formula" src="file://mIl5f2Ii.png" style="max-width: 100.0%;max-height: 100.0%;">, that aren't divisible by any hit indicator <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Recently, having fulfilled another quest, Igor K. found a new Lostborn sword. He wants to know how much damage he will inflict upon his enemies if he uses it.</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">13</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>). They are the indicator of Igor K's hero's strength and the number of hit indicators.</p><p>The next line contains space-separated <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). They are Lostborn sword's hit indicators. The given <span class="tex-span"><i>k</i></span> numbers are pairwise coprime.</p></div><div class="output-specification"><p>Print the single number — the damage that will be inflicted by Igor K.'s hero when he uses his new weapon. </p><p><span class="tex-font-style-bf">Please, do not use the %lld specificator to read or write 64-bit integers in C++. It is preferred to use the cin, cout streams or the %I64d specificator</span>.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">13</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>). They are the indicator of Igor K's hero's strength and the number of hit indicators.</p><p>The next line contains space-separated <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). They are Lostborn sword's hit indicators. The given <span class="tex-span"><i>k</i></span> numbers are pairwise coprime.</p>

## Output

<p>Print the single number — the damage that will be inflicted by Igor K.'s hero when he uses his new weapon. </p><p><span class="tex-font-style-bf">Please, do not use the %lld specificator to read or write 64-bit integers in C++. It is preferred to use the cin, cout streams or the %I64d specificator</span>.</p>





```input1
20 3
2 3 5

```




```input2
50 2
15 8

```




```output1
6

```




```output2
41

```


