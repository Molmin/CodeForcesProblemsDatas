## Description

<div><p>Today DZY begins to play an old game. In this game, he is in a big maze with <span class="tex-span"><i>n</i></span> rooms connected by <span class="tex-span"><i>m</i></span> corridors (each corridor allows to move in both directions). You can assume that all the rooms are connected with corridors directly or indirectly.</p><p>DZY has got lost in the maze. Currently he is in the first room and has <span class="tex-span"><i>k</i></span> lives. He will act like the follows:</p><ul> <li> Firstly he will randomly pick one of the corridors going from his current room. Each outgoing corridor has the same probability to be picked. </li><li> Then he will go through the corridor and then the process repeats. </li></ul><p>There are some rooms which have traps in them. The first room definitely has no trap, the <span class="tex-span"><i>n</i></span>-th room definitely has a trap. Each time DZY enters one of these rooms, he will lost one life. Now, DZY knows that if he enters the <span class="tex-span"><i>n</i></span>-th room with exactly 2 lives, firstly he will lost one live, but then he will open a bonus round. He wants to know the probability for him to open the bonus round. Please, help him.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>&nbsp;(2 ≤ <i>n</i> ≤ 500;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, each of them is either <span class="tex-span">0</span> or <span class="tex-span">1</span>. If the <span class="tex-span"><i>i</i></span>-th number is <span class="tex-span">1</span>, then the <span class="tex-span"><i>i</i></span>-th room has a trap, otherwise it has not a trap. <span class="tex-font-style-bf">Please note</span>, that the number of rooms with a trap is no more than <span class="tex-span">101</span>. It is guaranteed that the first room has no trap, and the <span class="tex-span"><i>n</i></span>-th room has a trap.</p><p>Then <span class="tex-span"><i>m</i></span> lines follows. Each of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>, meaning that current corridor connects two rooms <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the corridor system is connected.</p></div><div class="output-specification"><p>Print the only real number — the probability for DZY to open the bonus round. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>&nbsp;(2 ≤ <i>n</i> ≤ 500;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, each of them is either <span class="tex-span">0</span> or <span class="tex-span">1</span>. If the <span class="tex-span"><i>i</i></span>-th number is <span class="tex-span">1</span>, then the <span class="tex-span"><i>i</i></span>-th room has a trap, otherwise it has not a trap. <span class="tex-font-style-bf">Please note</span>, that the number of rooms with a trap is no more than <span class="tex-span">101</span>. It is guaranteed that the first room has no trap, and the <span class="tex-span"><i>n</i></span>-th room has a trap.</p><p>Then <span class="tex-span"><i>m</i></span> lines follows. Each of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>, meaning that current corridor connects two rooms <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the corridor system is connected.</p>

## Output

<p>Print the only real number — the probability for DZY to open the bonus round. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
5 5 3
0 0 1 0 1
1 2
2 3
3 4
4 5
1 2

```




```input2
3 2 2
0 1 1
1 2
2 3

```




```input3
2 1 3
0 1
1 2

```




```output1
0.25000000

```




```output2
-0.00000000

```




```output3
1.00000000

```


