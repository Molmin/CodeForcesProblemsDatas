## Description

<div><p>Furlo and Rublo play a game. The table has <span class="tex-span"><i>n</i></span> piles of coins lying on it, the <span class="tex-span"><i>i</i></span>-th pile has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> coins. Furlo and Rublo move in turns, Furlo moves first. In one move you are allowed to:</p><ul> <li> choose some pile, let's denote the current number of coins in it as <span class="tex-span"><i>x</i></span>; </li><li> choose some integer <span class="tex-span"><i>y</i></span> <span class="tex-span">(0 ≤ <i>y</i> &lt; <i>x</i>;&nbsp;<i>x</i><sup class="upper-index">1 / 4</sup> ≤ <i>y</i> ≤ <i>x</i><sup class="upper-index">1 / 2</sup>)</span> and decrease the number of coins in this pile to <span class="tex-span"><i>y</i></span>. In other words, after the described move the pile will have <span class="tex-span"><i>y</i></span> coins left. </li></ul><p>The player who can't make a move, loses. </p><p>Your task is to find out, who wins in the given game if both Furlo and Rublo play optimally well.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 77777)</span> — the number of piles. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 777777777777)</span> — the sizes of piles. The numbers are separated by single spaces.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>If both players play optimally well and Furlo wins, print "<span class="tex-font-style-tt">Furlo</span>", otherwise print "<span class="tex-font-style-tt">Rublo</span>". Print the answers without the quotes.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 77777)</span> — the number of piles. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 777777777777)</span> — the sizes of piles. The numbers are separated by single spaces.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>If both players play optimally well and Furlo wins, print "<span class="tex-font-style-tt">Furlo</span>", otherwise print "<span class="tex-font-style-tt">Rublo</span>". Print the answers without the quotes.</p>





```input1
1
1

```




```input2
2
1 2

```




```input3
10
1 2 3 4 5 6 7 8 9 10

```




```output1
Rublo

```




```output2
Rublo

```




```output3
Furlo

```


