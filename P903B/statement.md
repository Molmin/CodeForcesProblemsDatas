## Description

<div><p>Vova is again playing some computer game, now an RPG. In the game Vova's character received a quest: to slay the fearsome monster called Modcrab.</p><p>After two hours of playing the game Vova has tracked the monster and analyzed its tactics. The Modcrab has <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span> health points and an attack power of <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>. Knowing that, Vova has decided to buy a lot of strong healing potions and to prepare for battle.</p><p>Vova's character has <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span> health points and an attack power of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>. Also he has a large supply of healing potions, each of which increases his current amount of health points by <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> when Vova drinks a potion. All potions are identical to each other. It is guaranteed that <span class="tex-span"><i>c</i><sub class="lower-index">1</sub> &gt; <i>a</i><sub class="lower-index">2</sub></span>.</p><p>The battle consists of multiple phases. In the beginning of each phase, Vova can either attack the monster (thus reducing its health by <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>) or drink a healing potion (it increases Vova's health by <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>; <span class="tex-font-style-bf">Vova's health can exceed <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span></span>). Then, <span class="tex-font-style-bf">if the battle is not over yet</span>, the Modcrab attacks Vova, reducing his health by <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>. The battle ends when Vova's (or Modcrab's) health drops to <span class="tex-span">0</span> or lower. It is possible that the battle ends in a middle of a phase after Vova's attack.</p><p>Of course, Vova wants to win the fight. But also he wants to do it as fast as possible. So he wants to make up a strategy that will allow him to win the fight after the minimum possible number of phases.</p><p>Help Vova to make up a strategy! You may assume that Vova never runs out of healing potions, and that he can always win.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">1</sub> ≤ 100</span>, <span class="tex-span">2 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ 100</span>) — Vova's health, Vova's attack power and the healing power of a potion.</p><p>The second line contains two integers <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index">2</sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">2</sub> &lt; <i>c</i><sub class="lower-index">1</sub></span>) — the Modcrab's health and his attack power.</p></div><div class="output-specification"><p>In the first line print one integer <span class="tex-span"><i>n</i></span> denoting the minimum number of phases required to win the battle.</p><p>Then print <span class="tex-span"><i>n</i></span> lines. <span class="tex-span"><i>i</i></span>-th line must be equal to <span class="tex-font-style-tt">HEAL</span> if Vova drinks a potion in <span class="tex-span"><i>i</i></span>-th phase, or <span class="tex-font-style-tt">STRIKE</span> if he attacks the Modcrab.</p><p>The strategy must be valid: Vova's character must not be defeated before slaying the Modcrab, and the monster's health must be <span class="tex-span">0</span> or lower after Vova's last action.</p><p>If there are multiple optimal solutions, print any of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">1</sub> ≤ 100</span>, <span class="tex-span">2 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ 100</span>) — Vova's health, Vova's attack power and the healing power of a potion.</p><p>The second line contains two integers <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index">2</sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">2</sub> &lt; <i>c</i><sub class="lower-index">1</sub></span>) — the Modcrab's health and his attack power.</p>

## Output

<p>In the first line print one integer <span class="tex-span"><i>n</i></span> denoting the minimum number of phases required to win the battle.</p><p>Then print <span class="tex-span"><i>n</i></span> lines. <span class="tex-span"><i>i</i></span>-th line must be equal to <span class="tex-font-style-tt">HEAL</span> if Vova drinks a potion in <span class="tex-span"><i>i</i></span>-th phase, or <span class="tex-font-style-tt">STRIKE</span> if he attacks the Modcrab.</p><p>The strategy must be valid: Vova's character must not be defeated before slaying the Modcrab, and the monster's health must be <span class="tex-span">0</span> or lower after Vova's last action.</p><p>If there are multiple optimal solutions, print any of them.</p>





```input1
10 6 100
17 5

```




```input2
11 6 100
12 5

```




```output1
4
STRIKE
HEAL
STRIKE
STRIKE

```




```output2
2
STRIKE
STRIKE

```



## Note

<p>In the first example Vova's character must heal before or after his first attack. Otherwise his health will drop to zero in <span class="tex-span">2</span> phases while he needs <span class="tex-span">3</span> strikes to win.</p><p>In the second example no healing needed, two strikes are enough to get monster to zero health and win with <span class="tex-span">6</span> health left.</p>
