## Description

<div><p>A monster is attacking the Cyberland!</p><p>Master Yang, a braver, is going to beat the monster. Yang and the monster each have 3 attributes: hitpoints (<span class="tex-span"><i>HP</i></span>), offensive power (<span class="tex-span"><i>ATK</i></span>) and defensive power (<span class="tex-span"><i>DEF</i></span>).</p><p>During the battle, every second the monster's HP decrease by <span class="tex-span"><i>max</i>(0, <i>ATK</i><sub class="lower-index"><i>Y</i></sub> - <i>DEF</i><sub class="lower-index"><i>M</i></sub>)</span>, while Yang's HP decreases by <span class="tex-span"><i>max</i>(0, <i>ATK</i><sub class="lower-index"><i>M</i></sub> - <i>DEF</i><sub class="lower-index"><i>Y</i></sub>)</span>, where index <span class="tex-span"><i>Y</i></span> denotes Master Yang and index <span class="tex-span"><i>M</i></span> denotes monster. Both decreases happen simultaneously Once monster's <span class="tex-span"><i>HP</i> ≤ 0</span> and the same time Master Yang's <span class="tex-span"><i>HP</i> &gt; 0</span>, Master Yang wins.</p><p>Master Yang can buy attributes from the magic shop of Cyberland: <span class="tex-span"><i>h</i></span> bitcoins per <span class="tex-span"><i>HP</i></span>, <span class="tex-span"><i>a</i></span> bitcoins per <span class="tex-span"><i>ATK</i></span>, and <span class="tex-span"><i>d</i></span> bitcoins per <span class="tex-span"><i>DEF</i></span>.</p><p>Now Master Yang wants to know the minimum number of bitcoins he can spend in order to win.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>HP</i><sub class="lower-index"><i>Y</i></sub>, <i>ATK</i><sub class="lower-index"><i>Y</i></sub>, <i>DEF</i><sub class="lower-index"><i>Y</i></sub></span>, separated by a space, denoting the initial <span class="tex-span"><i>HP</i></span>, <span class="tex-span"><i>ATK</i></span> and <span class="tex-span"><i>DEF</i></span> of Master Yang.</p><p>The second line contains three integers <span class="tex-span"><i>HP</i><sub class="lower-index"><i>M</i></sub>, <i>ATK</i><sub class="lower-index"><i>M</i></sub>, <i>DEF</i><sub class="lower-index"><i>M</i></sub></span>, separated by a space, denoting the <span class="tex-span"><i>HP</i></span>, <span class="tex-span"><i>ATK</i></span> and <span class="tex-span"><i>DEF</i></span> of the monster.</p><p>The third line contains three integers <span class="tex-span"><i>h</i>, <i>a</i>, <i>d</i></span>, separated by a space, denoting the price of <span class="tex-span">1&nbsp;<i>HP</i></span>, <span class="tex-span">1&nbsp;<i>ATK</i></span> and <span class="tex-span">1&nbsp;<i>DEF</i></span>.</p><p>All numbers in input are <span class="tex-font-style-bf">integer</span> and lie between <span class="tex-span">1</span> and <span class="tex-span">100</span> inclusively.</p></div><div class="output-specification"><p>The only output line should contain an integer, denoting the minimum bitcoins Master Yang should spend in order to win.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>HP</i><sub class="lower-index"><i>Y</i></sub>, <i>ATK</i><sub class="lower-index"><i>Y</i></sub>, <i>DEF</i><sub class="lower-index"><i>Y</i></sub></span>, separated by a space, denoting the initial <span class="tex-span"><i>HP</i></span>, <span class="tex-span"><i>ATK</i></span> and <span class="tex-span"><i>DEF</i></span> of Master Yang.</p><p>The second line contains three integers <span class="tex-span"><i>HP</i><sub class="lower-index"><i>M</i></sub>, <i>ATK</i><sub class="lower-index"><i>M</i></sub>, <i>DEF</i><sub class="lower-index"><i>M</i></sub></span>, separated by a space, denoting the <span class="tex-span"><i>HP</i></span>, <span class="tex-span"><i>ATK</i></span> and <span class="tex-span"><i>DEF</i></span> of the monster.</p><p>The third line contains three integers <span class="tex-span"><i>h</i>, <i>a</i>, <i>d</i></span>, separated by a space, denoting the price of <span class="tex-span">1&nbsp;<i>HP</i></span>, <span class="tex-span">1&nbsp;<i>ATK</i></span> and <span class="tex-span">1&nbsp;<i>DEF</i></span>.</p><p>All numbers in input are <span class="tex-font-style-bf">integer</span> and lie between <span class="tex-span">1</span> and <span class="tex-span">100</span> inclusively.</p>

## Output

<p>The only output line should contain an integer, denoting the minimum bitcoins Master Yang should spend in order to win.</p>





```input1
1 2 1
1 100 1
1 100 100

```




```input2
100 100 100
1 1 1
1 1 1

```




```output1
99

```




```output2
0

```



## Note

<p>For the first sample, prices for <span class="tex-span"><i>ATK</i></span> and <span class="tex-span"><i>DEF</i></span> are extremely high. Master Yang can buy <span class="tex-span">99</span> HP, then he can beat the monster with <span class="tex-span">1</span> HP left.</p><p>For the second sample, Master Yang is strong enough to beat the monster, so he doesn't need to buy anything.</p>
