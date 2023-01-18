## Description

<div><p>Jeff has become friends with Furik. Now these two are going to play one quite amusing game.</p><p>At the beginning of the game Jeff takes a piece of paper and writes down a permutation consisting of <span class="tex-span"><i>n</i></span> numbers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub></span>. Then the guys take turns to make moves, Jeff moves first. During his move, Jeff chooses two adjacent permutation elements and then the boy swaps them. During his move, Furic tosses a coin and if the coin shows "heads" he chooses a random pair of adjacent elements with indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span>, for which an inequality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &gt; <i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> holds, and swaps them. But if the coin shows "tails", Furik chooses a random pair of adjacent elements with indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span>, for which the inequality <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> holds, and swaps them. If the coin shows "heads" or "tails" and Furik has multiple ways of adjacent pairs to take, then he uniformly takes one of the pairs. If Furik doesn't have any pair to take, he tosses a coin one more time. The game ends when the permutation is sorted in the increasing order.</p><p>Jeff wants the game to finish as quickly as possible (that is, he wants both players to make as few moves as possible). Help Jeff find the minimum mathematical expectation of the number of moves in the game if he moves optimally well.</p><p>You can consider that the coin shows the heads (or tails) with the probability of <span class="tex-span">50</span> percent.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3000)</span>. The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the permutation <span class="tex-span"><i>p</i></span>. The numbers are separated by spaces.</p></div><div class="output-specification"><p>In a single line print a single real value — the answer to the problem. The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3000)</span>. The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the permutation <span class="tex-span"><i>p</i></span>. The numbers are separated by spaces.</p>

## Output

<p>In a single line print a single real value — the answer to the problem. The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2
1 2

```




```input2
5
3 5 2 4 1

```




```output1
0.000000

```




```output2
13.000000

```



## Note

<p>In the first test the sequence is already sorted, so the answer is <span class="tex-span">0</span>.</p>
