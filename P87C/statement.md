## Description

<div><p>Two best friends Serozha and Gena play a game.</p><p>Initially there is one pile consisting of <span class="tex-span"><i>n</i></span> stones on the table. During one move one pile should be taken and divided into an arbitrary number of piles consisting of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> &gt; <i>a</i><sub class="lower-index">2</sub> &gt; ... &gt; <i>a</i><sub class="lower-index"><i>k</i></sub> &gt; 0</span> stones. The piles should meet the condition <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> - <i>a</i><sub class="lower-index">2</sub> = <i>a</i><sub class="lower-index">2</sub> - <i>a</i><sub class="lower-index">3</sub> = ... = <i>a</i><sub class="lower-index"><i>k</i> - 1</sub> - <i>a</i><sub class="lower-index"><i>k</i></sub> = 1</span>. Naturally, the number of piles <span class="tex-span"><i>k</i></span> should be no less than two.</p><p>The friends play in turns. The player who cannot make a move loses. Serozha makes the first move. Who will win if both players play in the optimal way?</p></div><div class="input-specification"><p>The single line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>If Serozha wins, print <span class="tex-span"><i>k</i></span>, which represents the minimal number of piles into which he can split the initial one during the first move in order to win the game.</p><p>If Gena wins, print "-1" (without the quotes).</p></div>

## Input

<p>The single line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>If Serozha wins, print <span class="tex-span"><i>k</i></span>, which represents the minimal number of piles into which he can split the initial one during the first move in order to win the game.</p><p>If Gena wins, print "-1" (without the quotes).</p>





```input1
3

```




```input2
6

```




```input3
100

```




```output1
2

```




```output2
-1

```




```output3
8

```


