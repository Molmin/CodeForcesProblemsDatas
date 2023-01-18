## Description

<div><p>Bananistan is a beautiful banana republic. Beautiful women in beautiful dresses. Beautiful statues of beautiful warlords. Beautiful stars in beautiful nights.</p><p>In Bananistan people play this crazy game – Bulbo. There’s an array of bulbs and player at the position, which represents one of the bulbs. The distance between two neighboring bulbs is 1. Before each turn player can change his position with cost <span class="tex-span">|<i>pos</i><sub class="lower-index"><i>new</i></sub> - <i>pos</i><sub class="lower-index"><i>old</i></sub>|</span>. After that, a contiguous set of bulbs lights-up and player pays the cost that’s equal to the distance to the closest shining bulb. Then, all bulbs go dark again. The goal is to minimize your summed cost. I tell you, Bananistanians are spending their nights playing with bulbs.</p><p>Banana day is approaching, and you are hired to play the most beautiful Bulbo game ever. A huge array of bulbs is installed, and you know your initial position and all the light-ups in advance. You need to play the ideal game and impress Bananistanians, and their families.</p></div><div class="input-specification"><p>The first line contains number of turns <span class="tex-span"><i>n</i></span> and initial position <span class="tex-span"><i>x</i></span>. Next <span class="tex-span"><i>n</i></span> lines contain two numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>start</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>end</i></sub></span>, which represent that all bulbs from interval <span class="tex-span">[<i>l</i><sub class="lower-index"><i>start</i></sub>, <i>l</i><sub class="lower-index"><i>end</i></sub>]</span> are shining this turn.</p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span> </li><li> <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span> </li><li> <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>start</i></sub> ≤ <i>l</i><sub class="lower-index"><i>end</i></sub> ≤ 10<sup class="upper-index">9</sup></span> </li></ul></div><div class="output-specification"><p>Output should contain a single number which represents the best result (minimum cost) that could be obtained by playing this Bulbo game.</p></div>

## Input

<p>The first line contains number of turns <span class="tex-span"><i>n</i></span> and initial position <span class="tex-span"><i>x</i></span>. Next <span class="tex-span"><i>n</i></span> lines contain two numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>start</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>end</i></sub></span>, which represent that all bulbs from interval <span class="tex-span">[<i>l</i><sub class="lower-index"><i>start</i></sub>, <i>l</i><sub class="lower-index"><i>end</i></sub>]</span> are shining this turn.</p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span> </li><li> <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span> </li><li> <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>start</i></sub> ≤ <i>l</i><sub class="lower-index"><i>end</i></sub> ≤ 10<sup class="upper-index">9</sup></span> </li></ul>

## Output

<p>Output should contain a single number which represents the best result (minimum cost) that could be obtained by playing this Bulbo game.</p>





```input1
5 4
2 7
9 16
8 10
9 17
1 6

```




```output1
8

```



## Note

<p>Before 1. turn move to position 5</p><p>Before 2. turn move to position 9</p><p>Before 5. turn move to position 8</p>
