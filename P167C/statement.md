## Description

<div><p>In some country live wizards. They love playing with numbers. </p><p>The blackboard has two numbers written on it — <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. The order of the numbers is not important. Let's consider <span class="tex-span"><i>a</i> ≤ <i>b</i></span> for the sake of definiteness. The players can cast one of the two spells in turns:</p><ul> <li> Replace <span class="tex-span"><i>b</i></span> with <span class="tex-span"><i>b</i> - <i>a</i><sup class="upper-index"><i>k</i></sup></span>. Number <span class="tex-span"><i>k</i></span> can be chosen by the player, considering the limitations that <span class="tex-span"><i>k</i> &gt; 0</span> and <span class="tex-span"><i>b</i> - <i>a</i><sup class="upper-index"><i>k</i></sup> ≥ 0</span>. Number <span class="tex-span"><i>k</i></span> is chosen independently each time an active player casts a spell. </li><li> Replace <span class="tex-span"><i>b</i></span> with <span class="tex-span"><i>b</i>&nbsp;<i>mod</i>&nbsp;<i>a</i></span>. </li></ul><p>If <span class="tex-span"><i>a</i> &gt; <i>b</i></span>, similar moves are possible.</p><p>If at least one of the numbers equals zero, a player can't make a move, because taking a remainder modulo zero is considered somewhat uncivilized, and it is far too boring to subtract a zero. The player who cannot make a move, loses.</p><p>To perform well in the magic totalizator, you need to learn to quickly determine which player wins, if both wizards play optimally: the one that moves first or the one that moves second.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>t</i></span> — the number of input data sets (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup></span>). Each of the next <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>). The numbers are separated by a space.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div><div class="output-specification"><p>For any of the <span class="tex-span"><i>t</i></span> input sets print "<span class="tex-font-style-tt">First</span>" (without the quotes) if the player who moves first wins. Print "<span class="tex-font-style-tt">Second</span>" (without the quotes) if the player who moves second wins. Print the answers to different data sets on different lines in the order in which they are given in the input. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>t</i></span> — the number of input data sets (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup></span>). Each of the next <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>). The numbers are separated by a space.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>

## Output

<p>For any of the <span class="tex-span"><i>t</i></span> input sets print "<span class="tex-font-style-tt">First</span>" (without the quotes) if the player who moves first wins. Print "<span class="tex-font-style-tt">Second</span>" (without the quotes) if the player who moves second wins. Print the answers to different data sets on different lines in the order in which they are given in the input. </p>





```input1
4
10 21
31 10
0 1
10 30

```




```output1
First
Second
Second
First

```



## Note

<p>In the first sample, the first player should go to (11,10). Then, after a single move of the second player to (1,10), he will take 10 modulo 1 and win.</p><p>In the second sample the first player has two moves to (1,10) and (21,10). After both moves the second player can win.</p><p>In the third sample, the first player has no moves.</p><p>In the fourth sample, the first player wins in one move, taking 30 modulo 10.</p>
