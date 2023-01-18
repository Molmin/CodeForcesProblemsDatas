## Description

<div><p>Mishka is decorating the Christmas tree. He has got three garlands, and all of them will be put on the tree. After that Mishka will switch these garlands on.</p><p>When a garland is switched on, it periodically changes its state — sometimes it is lit, sometimes not. Formally, if <span class="tex-span"><i>i</i></span>-th garland is switched on during <span class="tex-span"><i>x</i></span>-th second, then it is lit only during seconds <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>x</i> + <i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i> + 2<i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i> + 3<i>k</i><sub class="lower-index"><i>i</i></sub></span> and so on.</p><p>Mishka wants to switch on the garlands in such a way that during each second after switching the garlands on there would be at least one lit garland. Formally, Mishka wants to choose three integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span> (not necessarily distinct) so that he will switch on the first garland during <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>-th second, the second one — during <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>-th second, and the third one — during <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span>-th second, respectively, and during each second starting from <span class="tex-span"><i>max</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>)</span> at least one garland will be lit.</p><p>Help Mishka by telling him if it is possible to do this!</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 1500</span>) — time intervals of the garlands.</p></div><div class="output-specification"><p>If Mishka can choose moments of time to switch on the garlands in such a way that each second after switching the garlands on at least one garland will be lit, print <span class="tex-font-style-tt">YES</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 1500</span>) — time intervals of the garlands.</p>

## Output

<p>If Mishka can choose moments of time to switch on the garlands in such a way that each second after switching the garlands on at least one garland will be lit, print <span class="tex-font-style-tt">YES</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
2 2 3

```




```input2
4 2 3

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first example Mishka can choose <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> = 2</span>, <span class="tex-span"><i>x</i><sub class="lower-index">3</sub> = 1</span>. The first garland will be lit during seconds <span class="tex-span">1, 3, 5, 7, ...</span>, the second — <span class="tex-span">2, 4, 6, 8, ...</span>, which already cover all the seconds after the <span class="tex-span">2</span>-nd one. It doesn't even matter what <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span> is chosen. Our choice will lead third to be lit during seconds <span class="tex-span">1, 4, 7, 10, ...</span>, though.</p><p>In the second example there is no way to choose such moments of time, there always be some seconds when no garland is lit.</p>
