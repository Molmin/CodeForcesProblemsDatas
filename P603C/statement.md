## Description

<div><p>Kevin and Nicky Sun have invented a new game called Lieges of Legendre. In this game, two players take turns modifying the game state with Kevin moving first. Initially, the game is set up so that there are <span class="tex-span"><i>n</i></span> piles of cows, with the <span class="tex-span"><i>i</i></span>-th pile containing <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> cows. During each player's turn, that player calls upon the power of Sunlight, and uses it to either:</p><ol> <li> Remove a single cow from a chosen non-empty pile. </li><li> Choose a pile of cows with even size <span class="tex-span">2·<i>x</i></span> (<span class="tex-span"><i>x</i> &gt; 0</span>), and replace it with <span class="tex-span"><i>k</i></span> piles of <span class="tex-span"><i>x</i></span> cows each. </li></ol><p>The player who removes the last cow wins. Given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, and a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, help Kevin and Nicky find the winner, given that both sides play in optimal way.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) describing the initial state of the game. </p></div><div class="output-specification"><p>Output the name of the winning player, either "<span class="tex-font-style-tt">Kevin</span>" or "<span class="tex-font-style-tt">Nicky</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) describing the initial state of the game. </p>

## Output

<p>Output the name of the winning player, either "<span class="tex-font-style-tt">Kevin</span>" or "<span class="tex-font-style-tt">Nicky</span>" (without quotes).</p>





```input1
2 1
3 4

```




```input2
1 2
3

```




```output1
Kevin

```




```output2
Nicky

```



## Note

<p>In the second sample, Nicky can win in the following way: Kevin moves first and is forced to remove a cow, so the pile contains two cows after his move. Next, Nicky replaces this pile of size 2 with two piles of size 1. So the game state is now two piles of size 1. Kevin then removes one of the remaining cows and Nicky wins by removing the other.</p>
