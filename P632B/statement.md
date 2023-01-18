## Description

<div><p>Alice and Bob are playing a game. The game involves splitting up game pieces into two teams. There are <span class="tex-span"><i>n</i></span> pieces, and the <span class="tex-span"><i>i</i></span>-th piece has a strength <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The way to split up game pieces is split into several steps:</p><ol> <li> First, Alice will split the pieces into two different groups <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>. This can be seen as writing the assignment of teams of a piece in an <span class="tex-span"><i>n</i></span> character string, where each character is <span class="tex-span"><i>A</i></span> or <span class="tex-span"><i>B</i></span>. </li><li> Bob will then choose an arbitrary prefix or suffix of the string, and flip each character in that suffix (i.e. change <span class="tex-span"><i>A</i></span> to <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>B</i></span> to <span class="tex-span"><i>A</i></span>). He can do this step at most once. </li><li> Alice will get all the pieces marked <span class="tex-span"><i>A</i></span> and Bob will get all the pieces marked <span class="tex-span"><i>B</i></span>. </li></ol><p>The strength of a player is then the sum of strengths of the pieces in the group.</p><p>Given Alice's initial split into two teams, help Bob determine an optimal strategy. Return the maximum strength he can achieve.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of game pieces.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the strength of the <span class="tex-span"><i>i</i></span>-th piece.</p><p>The third line contains <span class="tex-span"><i>n</i></span> characters <span class="tex-span"><i>A</i></span> or <span class="tex-span"><i>B</i></span> — the assignment of teams after the first step (after Alice's step).</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>a</i></span> — the maximum strength Bob can achieve.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of game pieces.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the strength of the <span class="tex-span"><i>i</i></span>-th piece.</p><p>The third line contains <span class="tex-span"><i>n</i></span> characters <span class="tex-span"><i>A</i></span> or <span class="tex-span"><i>B</i></span> — the assignment of teams after the first step (after Alice's step).</p>

## Output

<p>Print the only integer <span class="tex-span"><i>a</i></span> — the maximum strength Bob can achieve.</p>





```input1
5
1 2 3 4 5
ABABA

```




```input2
5
1 2 3 4 5
AAAAA

```




```input3
1
1
B

```




```output1
11

```




```output2
15

```




```output3
1

```



## Note

<p>In the first sample Bob should flip the suffix of length one.</p><p>In the second sample Bob should flip the prefix or the suffix (here it is the same) of length <span class="tex-span">5</span>.</p><p>In the third sample Bob should do nothing.</p>
