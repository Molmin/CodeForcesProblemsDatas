## Description

<div><p>As you might remember from the previous round, Vova is currently playing a strategic game known as Rage of Empires.</p><p>Vova managed to build a large army, but forgot about the main person in the army - the commander. So he tries to hire a commander, and he wants to choose the person who will be respected by warriors.</p><p>Each warrior is represented by his personality — an integer number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Each commander has two characteristics — his personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> and leadership <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> (both are integer numbers). Warrior <span class="tex-span"><i>i</i></span> <span class="tex-font-style-it">respects</span> commander <span class="tex-span"><i>j</i></span> only if <img align="middle" class="tex-formula" src="file://Zv8Hwqb5.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="file://lvEYkk5t.png" style="max-width: 100.0%;max-height: 100.0%;"> is the bitwise excluding OR of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>).</p><p>Initially Vova's army is empty. There are three different types of events that can happen with the army:</p><ul> <li> <span class="tex-span">1&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub></span> — one warrior with personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> joins Vova's army; </li><li> <span class="tex-span">2&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub></span> — one warrior with personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> leaves Vova's army; </li><li> <span class="tex-span">3&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>l</i><sub class="lower-index"><i>i</i></sub></span> — Vova tries to hire a commander with personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and leadership <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul><p>For each event of the third type Vova wants to know how many warriors (counting only those who joined the army and haven't left yet) <span class="tex-font-style-it">respect</span> the commander he tries to hire.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100000</span>) — the number of events.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. Each line describes the event:</p><ul> <li> <span class="tex-span">1&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — one warrior with personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> joins Vova's army; </li><li> <span class="tex-span">2&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — one warrior with personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> leaves Vova's army (it is guaranteed that there is at least one such warrior in Vova's army by this moment); </li><li> <span class="tex-span">3&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — Vova tries to hire a commander with personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and leadership <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>. There is at least one event of this type. </li></ul></div><div class="output-specification"><p>For each event of the third type print one integer — the number of warriors who <span class="tex-font-style-it">respect</span> the commander Vova tries to hire in the event.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100000</span>) — the number of events.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. Each line describes the event:</p><ul> <li> <span class="tex-span">1&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — one warrior with personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> joins Vova's army; </li><li> <span class="tex-span">2&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — one warrior with personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> leaves Vova's army (it is guaranteed that there is at least one such warrior in Vova's army by this moment); </li><li> <span class="tex-span">3&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — Vova tries to hire a commander with personality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and leadership <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>. There is at least one event of this type. </li></ul>

## Output

<p>For each event of the third type print one integer — the number of warriors who <span class="tex-font-style-it">respect</span> the commander Vova tries to hire in the event.</p>





```input1
5
1 3
1 4
3 6 3
2 4
3 6 3

```




```output1
1
0

```



## Note

<p>In the example the army consists of two warriors with personalities <span class="tex-span">3</span> and <span class="tex-span">4</span> after first two events. Then Vova tries to hire a commander with personality <span class="tex-span">6</span> and leadership <span class="tex-span">3</span>, and only one warrior respects him (<img align="middle" class="tex-formula" src="file://EcG60vgX.png" style="max-width: 100.0%;max-height: 100.0%;">, and <span class="tex-span">2 &lt; 3</span>, but <img align="middle" class="tex-formula" src="file://MgQCgsSo.png" style="max-width: 100.0%;max-height: 100.0%;">, and <span class="tex-span">5 ≥ 3</span>). Then warrior with personality <span class="tex-span">4</span> leaves, and when Vova tries to hire that commander again, there are no warriors who respect him.</p>
