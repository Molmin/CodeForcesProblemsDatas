## Description

<div><p>Little Petya likes permutations a lot. Recently his mom has presented him permutation <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span>.</p><p>A <span class="tex-font-style-it">permutation</span> <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span> is a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, all integers there are distinct. </p><p>There is only one thing Petya likes more than permutations: playing with little Masha. As it turns out, Masha also has a permutation of length <span class="tex-span"><i>n</i></span>. Petya decided to get the same permutation, whatever the cost may be. For that, he devised a game with the following rules:</p><ul> <li> Before the beginning of the game Petya writes permutation <span class="tex-span">1, 2, ..., <i>n</i></span> on the blackboard. After that Petya makes exactly <span class="tex-span"><i>k</i></span> moves, which are described below. </li><li> During a move Petya tosses a coin. If the coin shows heads, he performs point 1, if the coin shows tails, he performs point 2.<ol> <li> Let's assume that the board contains permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> at the given moment. Then Petya removes the written permutation <span class="tex-span"><i>p</i></span> from the board and writes another one instead: <span class="tex-span"><i>p</i><sub class="lower-index"><i>q</i><sub class="lower-index">1</sub></sub>, <i>p</i><sub class="lower-index"><i>q</i><sub class="lower-index">2</sub></sub>, ..., <i>p</i><sub class="lower-index"><i>q</i><sub class="lower-index"><i>n</i></sub></sub></span>. In other words, Petya applies permutation <span class="tex-span"><i>q</i></span> (which he has got from his mother) to permutation <span class="tex-span"><i>p</i></span>. </li><li> All actions are similar to point 1, except that Petya writes permutation <span class="tex-span"><i>t</i></span> on the board, such that: <span class="tex-span"><i>t</i><sub class="lower-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sub> = <i>p</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>n</i></span>. In other words, Petya applies a permutation that is inverse to <span class="tex-span"><i>q</i></span> to permutation <span class="tex-span"><i>p</i></span>. </li></ol></li></ul><p>We know that after the <span class="tex-span"><i>k</i></span>-th move the board contained Masha's permutation <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span>. Besides, we know that throughout the game process Masha's permutation <span class="tex-font-style-bf">never occurred on the board</span> before the <span class="tex-span"><i>k</i></span>-th move. Note that the game has exactly <span class="tex-span"><i>k</i></span> moves, that is, throughout the game the coin was tossed exactly <span class="tex-span"><i>k</i></span> times.</p><p>Your task is to determine whether the described situation is possible or else state that Petya was mistaken somewhere. See samples and notes to them for a better understanding.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the permutation that Petya's got as a present. The third line contains Masha's permutation <span class="tex-span"><i>s</i></span>, in the similar format.</p><p>It is guaranteed that the given sequences <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>s</i></span> are correct permutations.</p></div><div class="output-specification"><p>If the situation that is described in the statement is possible, print "<span class="tex-font-style-tt">YES</span>" (without the quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the permutation that Petya's got as a present. The third line contains Masha's permutation <span class="tex-span"><i>s</i></span>, in the similar format.</p><p>It is guaranteed that the given sequences <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>s</i></span> are correct permutations.</p>

## Output

<p>If the situation that is described in the statement is possible, print "<span class="tex-font-style-tt">YES</span>" (without the quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
4 1
2 3 4 1
1 2 3 4

```




```input2
4 1
4 3 1 2
3 4 2 1

```




```input3
4 3
4 3 1 2
3 4 2 1

```




```input4
4 2
4 3 1 2
2 1 4 3

```




```input5
4 1
4 3 1 2
2 1 4 3

```




```output1
NO

```




```output2
YES

```




```output3
YES

```




```output4
YES

```




```output5
NO

```



## Note

<p>In the first sample Masha's permutation coincides with the permutation that was written on the board before the beginning of the game. Consequently, that violates the condition that Masha's permutation never occurred on the board before <span class="tex-span"><i>k</i></span> moves were performed.</p><p>In the second sample the described situation is possible, in case if after we toss a coin, we get tails.</p><p>In the third sample the possible coin tossing sequence is: heads-tails-tails.</p><p>In the fourth sample the possible coin tossing sequence is: heads-heads.</p>
