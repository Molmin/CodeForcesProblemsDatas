## Description

<div><p>User ainta loves to play with cards. He has <span class="tex-span"><i>a</i></span> cards containing letter "<span class="tex-font-style-tt">o</span>" and <span class="tex-span"><i>b</i></span> cards containing letter "<span class="tex-font-style-tt">x</span>". He arranges the cards in a row, and calculates the score of the deck by the formula below.</p><ol> <li> At first, the score is <span class="tex-span">0</span>. </li><li> For each block of contiguous "<span class="tex-font-style-tt">o</span>"s with length <span class="tex-span"><i>x</i></span> the score increases by <span class="tex-span"><i>x</i><sup class="upper-index">2</sup></span>. </li><li> For each block of contiguous "<span class="tex-font-style-tt">x</span>"s with length <span class="tex-span"><i>y</i></span> the score decreases by <span class="tex-span"><i>y</i><sup class="upper-index">2</sup></span>. </li></ol> &nbsp;<p>For example, if <span class="tex-span"><i>a</i> = 6, <i>b</i> = 3</span> and ainta have arranged the cards in the order, that is described by string "<span class="tex-font-style-tt">ooxoooxxo</span>", the score of the deck equals <span class="tex-span">2<sup class="upper-index">2</sup> - 1<sup class="upper-index">2</sup> + 3<sup class="upper-index">2</sup> - 2<sup class="upper-index">2</sup> + 1<sup class="upper-index">2</sup> = 9</span>. That is because the deck has 5 blocks in total: "<span class="tex-font-style-tt">oo</span>", "<span class="tex-font-style-tt">x</span>", "<span class="tex-font-style-tt">ooo</span>", "<span class="tex-font-style-tt">xx</span>", "<span class="tex-font-style-tt">o</span>".</p><p>User ainta likes big numbers, so he wants to maximize the score with the given cards. Help ainta make the score as big as possible. Note, that he has to arrange all his cards.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;<i>a</i> + <i>b</i> ≥ 1</span>) — the number of "<span class="tex-font-style-tt">o</span>" cards and the number of "<span class="tex-font-style-tt">x</span>" cards.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>v</i></span> — the maximum score that ainta can obtain.</p><p>In the second line print <span class="tex-span"><i>a</i> + <i>b</i></span> characters describing the deck. If the <span class="tex-span"><i>k</i></span>-th card of the deck contains "<span class="tex-font-style-tt">o</span>", the <span class="tex-span"><i>k</i></span>-th character must be "<span class="tex-font-style-tt">o</span>". If the <span class="tex-span"><i>k</i></span>-th card of the deck contains "<span class="tex-font-style-tt">x</span>", the <span class="tex-span"><i>k</i></span>-th character must be "<span class="tex-font-style-tt">x</span>". The number of "<span class="tex-font-style-tt">o</span>" characters must be equal to <span class="tex-span"><i>a</i></span>, and the number of "<span class="tex-font-style-tt">x</span> " characters must be equal to <span class="tex-span"><i>b</i></span>. If there are many ways to maximize <span class="tex-span"><i>v</i></span>, print any.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;<i>a</i> + <i>b</i> ≥ 1</span>) — the number of "<span class="tex-font-style-tt">o</span>" cards and the number of "<span class="tex-font-style-tt">x</span>" cards.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>v</i></span> — the maximum score that ainta can obtain.</p><p>In the second line print <span class="tex-span"><i>a</i> + <i>b</i></span> characters describing the deck. If the <span class="tex-span"><i>k</i></span>-th card of the deck contains "<span class="tex-font-style-tt">o</span>", the <span class="tex-span"><i>k</i></span>-th character must be "<span class="tex-font-style-tt">o</span>". If the <span class="tex-span"><i>k</i></span>-th card of the deck contains "<span class="tex-font-style-tt">x</span>", the <span class="tex-span"><i>k</i></span>-th character must be "<span class="tex-font-style-tt">x</span>". The number of "<span class="tex-font-style-tt">o</span>" characters must be equal to <span class="tex-span"><i>a</i></span>, and the number of "<span class="tex-font-style-tt">x</span> " characters must be equal to <span class="tex-span"><i>b</i></span>. If there are many ways to maximize <span class="tex-span"><i>v</i></span>, print any.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
2 3

```




```input2
4 0

```




```input3
0 4

```




```output1
-1
xoxox

```




```output2
16
oooo
```




```output3
-16
xxxx
```


