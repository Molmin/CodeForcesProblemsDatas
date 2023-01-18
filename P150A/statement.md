## Description

<div><p>You can't possibly imagine how cold our friends are this winter in Nvodsk! Two of them play the following game to warm up: initially a piece of paper has an integer <span class="tex-span"><i>q</i></span>. During a move a player should write any integer number that is a <span class="tex-font-style-underline">non-trivial</span> divisor of the last written number. Then he should run this number of circles around the hotel. Let us remind you that a number's divisor is called <span class="tex-font-style-underline">non-trivial</span> if it is different from one and from the divided number itself. </p><p>The first person who <span class="tex-font-style-bf">can't make a move wins</span> as he continues to lie in his warm bed under three blankets while the other one keeps running. Determine which player wins considering that both players play optimally. If the first player wins, print any winning first move.</p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">13</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div><div class="output-specification"><p>In the first line print the number of the winning player (<span class="tex-span">1</span> or <span class="tex-span">2</span>). If the first player wins then the second line should contain another integer — his first move (if the first player can't even make the first move, print <span class="tex-span">0</span>). If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains the only integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">13</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>

## Output

<p>In the first line print the number of the winning player (<span class="tex-span">1</span> or <span class="tex-span">2</span>). If the first player wins then the second line should contain another integer — his first move (if the first player can't even make the first move, print <span class="tex-span">0</span>). If there are multiple solutions, print any of them.</p>





```input1
6

```




```input2
30

```




```input3
1

```




```output1
2

```




```output2
1
6

```




```output3
1
0

```



## Note

<p>Number <span class="tex-span">6</span> has only two non-trivial divisors: <span class="tex-span">2</span> and <span class="tex-span">3</span>. It is impossible to make a move after the numbers <span class="tex-span">2</span> and <span class="tex-span">3</span> are written, so both of them are winning, thus, number <span class="tex-span">6</span> is the losing number. A player can make a move and write number <span class="tex-span">6</span> after number <span class="tex-span">30</span>; <span class="tex-span">6</span>, as we know, is a losing number. Thus, this move will bring us the victory.</p>
