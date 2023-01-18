## Description

<div><p>Polycarp is in really serious trouble — his house is on fire! It's time to save the most valuable items. Polycarp estimated that it would take <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> seconds to save <span class="tex-span"><i>i</i></span>-th item. In addition, for each item, he estimated the value of <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> — the moment after which the item <span class="tex-span"><i>i</i></span> will be completely burned and will no longer be valuable for him at all. In particular, if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> ≥ <i>d</i><sub class="lower-index"><i>i</i></sub></span>, then <span class="tex-span"><i>i</i></span>-th item cannot be saved.</p><p>Given the values <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> for each of the items, find a set of items that Polycarp can save such that the total value of this items is maximum possible. Polycarp saves the items one after another. For example, if he takes item <span class="tex-span"><i>a</i></span> first, and then item <span class="tex-span"><i>b</i></span>, then the item <span class="tex-span"><i>a</i></span> will be saved in <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub></span> seconds, and the item <span class="tex-span"><i>b</i></span> — in <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub> + <i>t</i><sub class="lower-index"><i>b</i></sub></span> seconds after fire started.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of items in Polycarp's house.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 2 000</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>) — the time needed to save the item <span class="tex-span"><i>i</i></span>, the time after which the item <span class="tex-span"><i>i</i></span> will burn completely and the value of item <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>In the first line print the maximum possible total value of the set of saved items. In the second line print one integer <span class="tex-span"><i>m</i></span> — the number of items in the desired set. In the third line print <span class="tex-span"><i>m</i></span> distinct integers — numbers of the saved items <span class="tex-font-style-it">in the order Polycarp saves them</span>. Items are 1-indexed in the same order in which they appear in the input. If there are several answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of items in Polycarp's house.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 2 000</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>) — the time needed to save the item <span class="tex-span"><i>i</i></span>, the time after which the item <span class="tex-span"><i>i</i></span> will burn completely and the value of item <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>In the first line print the maximum possible total value of the set of saved items. In the second line print one integer <span class="tex-span"><i>m</i></span> — the number of items in the desired set. In the third line print <span class="tex-span"><i>m</i></span> distinct integers — numbers of the saved items <span class="tex-font-style-it">in the order Polycarp saves them</span>. Items are 1-indexed in the same order in which they appear in the input. If there are several answers, print any of them.</p>





```input1
3
3 7 4
2 6 5
3 7 6

```




```input2
2
5 6 1
3 3 5

```




```output1
11
2
2 3 

```




```output2
1
1
1 

```



## Note

<p>In the first example Polycarp will have time to save any two items, but in order to maximize the total value of the saved items, he must save the second and the third item. For example, he can firstly save the third item in <span class="tex-span">3</span> seconds, and then save the second item in another <span class="tex-span">2</span> seconds. Thus, the total value of the saved items will be <span class="tex-span">6 + 5 = 11</span>.</p><p>In the second example Polycarp can save only the first item, since even if he immediately starts saving the second item, he can save it in <span class="tex-span">3</span> seconds, but this item will already be completely burned by this time.</p>
