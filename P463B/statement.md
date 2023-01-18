## Description

<div><p>Caisa solved the problem with the sugar and now he is on the way back to home. </p><p>Caisa is playing a mobile game during his path. There are <span class="tex-span">(<i>n</i> + 1)</span> pylons numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span> in this game. The pylon with number <span class="tex-span">0</span> has zero height, the pylon with number <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>i</i> &gt; 0)</span> has height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. The goal of the game is to reach <span class="tex-span"><i>n</i></span>-th pylon, and the only move the player can do is to jump from the current pylon (let's denote its number as <span class="tex-span"><i>k</i></span>) to the next one (its number will be <span class="tex-span"><i>k</i> + 1</span>). When the player have made such a move, its energy increases by <span class="tex-span"><i>h</i><sub class="lower-index"><i>k</i></sub> - <i>h</i><sub class="lower-index"><i>k</i> + 1</sub></span> (if this value is negative the player loses energy). The player must have non-negative amount of energy at any moment of the time. </p><p>Initially Caisa stand at <span class="tex-span">0</span> pylon and has <span class="tex-span">0</span> energy. The game provides a special opportunity: one can pay a single dollar and increase the height of anyone pylon by one. Caisa may use that opportunity several times, but he doesn't want to spend too much money. What is the minimal amount of money he must paid to reach the goal of the game?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>h</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1  ≤  <i>h</i><sub class="lower-index"><i>i</i></sub>  ≤  10<sup class="upper-index">5</sup>)</span> representing the heights of the pylons.</p></div><div class="output-specification"><p>Print a single number representing the minimum number of dollars paid by Caisa.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>h</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1  ≤  <i>h</i><sub class="lower-index"><i>i</i></sub>  ≤  10<sup class="upper-index">5</sup>)</span> representing the heights of the pylons.</p>

## Output

<p>Print a single number representing the minimum number of dollars paid by Caisa.</p>





```input1
5
3 4 3 2 4

```




```input2
3
4 4 4

```




```output1
4

```




```output2
4

```



## Note

<p>In the first sample he can pay <span class="tex-span">4</span> dollars and increase the height of pylon with number <span class="tex-span">0</span> by <span class="tex-span">4</span> units. Then he can safely pass to the last pylon.</p>
