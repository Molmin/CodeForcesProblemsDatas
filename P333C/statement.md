## Description

<div><p>Gerald has a friend, Pollard. Pollard is interested in lucky tickets (ticket is a sequence of digits). At first he thought that a ticket is lucky if between some its digits we can add arithmetic signs and brackets so that the result obtained by the arithmetic expression was number 100. But he quickly analyzed all such tickets and moved on to a more general question. Now he explores <span class="tex-span"><i>k</i></span>-lucky tickets.</p><p>Pollard sais that a ticket is <span class="tex-span"><i>k</i></span>-lucky if we can add arithmetic operation signs between its digits to the left or right of them (i.e., "+", "-", "<span class="tex-span"> × </span>") and brackets so as to obtain the correct arithmetic expression whose value would equal <span class="tex-span"><i>k</i></span>. For example, ticket "224201016" is 1000-lucky as <span class="tex-span">( - 2 - (2 + 4)) × (2 + 0) + 1016 = 1000</span>.</p><p>Pollard was so carried away by the lucky tickets that he signed up for a seminar on lucky tickets and, as far as Gerald knows, Pollard will attend it daily at 7 pm in some famous institute and will commute to it in the same tram for <span class="tex-span"><i>m</i></span> days. In this tram tickets have eight digits. And Gerald wants to make a surprise for Pollard: each day Pollard will receive a tram <span class="tex-span"><i>k</i></span>-lucky ticket. The conductor has already agreed to give Pollard certain tickets during all these <span class="tex-span"><i>m</i></span> days and he only wants Gerald to tell him what kind of tickets to give out. In this regard, help Gerald pick exactly <span class="tex-span"><i>m</i></span> distinct <span class="tex-span"><i>k</i></span>-lucky tickets.</p></div><div class="input-specification"><p>The single line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. Each line must contain exactly 8 digits — the <span class="tex-span"><i>k</i></span>-winning ticket. The tickets may begin with 0, all tickets must be distinct. If there are more than <span class="tex-span"><i>m</i></span> distinct <span class="tex-span"><i>k</i></span>-lucky tickets, print any <span class="tex-span"><i>m</i></span> of them. It is guaranteed that at least <span class="tex-span"><i>m</i></span> distinct <span class="tex-span"><i>k</i></span>-lucky tickets exist. The tickets can be printed in any order.</p></div>

## Input

<p>The single line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. Each line must contain exactly 8 digits — the <span class="tex-span"><i>k</i></span>-winning ticket. The tickets may begin with 0, all tickets must be distinct. If there are more than <span class="tex-span"><i>m</i></span> distinct <span class="tex-span"><i>k</i></span>-lucky tickets, print any <span class="tex-span"><i>m</i></span> of them. It is guaranteed that at least <span class="tex-span"><i>m</i></span> distinct <span class="tex-span"><i>k</i></span>-lucky tickets exist. The tickets can be printed in any order.</p>





```input1
0 3

```




```input2
7 4

```




```output1
00000000
00000001
00000002

```




```output2
00000007
00000016
00000017
00000018

```


