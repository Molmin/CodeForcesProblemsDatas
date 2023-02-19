## Description

<div><p>Jon Snow is on the lookout for some orbs required to defeat the white walkers. There are <span class="tex-span"><i>k</i></span> different types of orbs and he needs at least one of each. One orb spawns daily at the base of a Weirwood tree north of the wall. The probability of this orb being of any kind is equal. As the north of wall is full of dangers, he wants to know the minimum number of days he should wait before sending a ranger to collect the orbs such that the probability of him getting at least one of each kind of orb is at least <img align="middle" class="tex-formula" src="file://3I5OBFuG.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span">ε &lt; 10<sup class="upper-index"> - 7</sup></span>.</p><p>To better prepare himself, he wants to know the answer for <span class="tex-span"><i>q</i></span> different values of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Since he is busy designing the battle strategy with Sam, he asks you for your help.</p></div><div class="input-specification"><p>First line consists of two space separated integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>k</i>, <i>q</i> ≤ 1000</span>) — number of different kinds of orbs and number of queries respectively.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contain a single integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> lines. On <span class="tex-span"><i>i</i></span>-th of them output single integer — answer for <span class="tex-span"><i>i</i></span>-th query.</p></div>

## Input

<p>First line consists of two space separated integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>k</i>, <i>q</i> ≤ 1000</span>) — number of different kinds of orbs and number of queries respectively.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contain a single integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> lines. On <span class="tex-span"><i>i</i></span>-th of them output single integer — answer for <span class="tex-span"><i>i</i></span>-th query.</p>





```input1
1 1
1

```




```input2
2 2
1
2

```




```output1
1

```




```output2
2
2

```


