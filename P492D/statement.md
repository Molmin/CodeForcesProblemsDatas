## Description

<div><p>Vanya and his friend Vova play a computer game where they need to destroy <span class="tex-span"><i>n</i></span> monsters to pass a level. Vanya's character performs attack with frequency <span class="tex-span"><i>x</i></span> hits per second and Vova's character performs attack with frequency <span class="tex-span"><i>y</i></span> hits per second. Each character spends fixed time to raise a weapon and then he hits (the time to raise the weapon is <span class="tex-span">1 / <i>x</i></span> seconds for the first character and <span class="tex-span">1 / <i>y</i></span> seconds for the second one). The <span class="tex-span"><i>i</i></span>-th monster dies after he receives <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> hits. </p><p>Vanya and Vova wonder who makes the last hit on each monster. If Vanya and Vova make the last hit at the same time, we assume that both of them have made the last hit.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>,<span class="tex-span"><i>x</i></span>,<span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of monsters, the frequency of Vanya's and Vova's attack, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of hits needed do destroy the <span class="tex-span"><i>i</i></span>-th monster.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print word "<span class="tex-font-style-tt">Vanya</span>", if the last hit on the <span class="tex-span"><i>i</i></span>-th monster was performed by Vanya, "<span class="tex-font-style-tt">Vova</span>", if Vova performed the last hit, or "<span class="tex-font-style-tt">Both</span>", if both boys performed it at the same time.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>,<span class="tex-span"><i>x</i></span>,<span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of monsters, the frequency of Vanya's and Vova's attack, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of hits needed do destroy the <span class="tex-span"><i>i</i></span>-th monster.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print word "<span class="tex-font-style-tt">Vanya</span>", if the last hit on the <span class="tex-span"><i>i</i></span>-th monster was performed by Vanya, "<span class="tex-font-style-tt">Vova</span>", if Vova performed the last hit, or "<span class="tex-font-style-tt">Both</span>", if both boys performed it at the same time.</p>





```input1
4 3 2
1
2
3
4

```




```input2
2 1 1
1
2

```




```output1
Vanya
Vova
Vanya
Both

```




```output2
Both
Both

```



## Note

<p>In the first sample Vanya makes the first hit at time <span class="tex-span">1 / 3</span>, Vova makes the second hit at time <span class="tex-span">1 / 2</span>, Vanya makes the third hit at time <span class="tex-span">2 / 3</span>, and both boys make the fourth and fifth hit simultaneously at the time <span class="tex-span">1</span>.</p><p>In the second sample Vanya and Vova make the first and second hit simultaneously at time <span class="tex-span">1</span>.</p>
