## Description

<div><p>One day <span class="tex-span"><i>n</i></span> friends gathered together to play "Mafia". During each round of the game some player must be the supervisor and other <span class="tex-span"><i>n</i> - 1</span> people take part in the game. For each person we know in how many rounds he wants to be a player, not the supervisor: the <span class="tex-span"><i>i</i></span>-th person wants to play <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> rounds. What is the minimum number of rounds of the "Mafia" game they need to play to let each person play at least as many rounds as they want?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th number in the list is the number of rounds the <span class="tex-span"><i>i</i></span>-th person wants to play.</p></div><div class="output-specification"><p>In a single line print a single integer — the minimum number of game rounds the friends need to let the <span class="tex-span"><i>i</i></span>-th person play at least <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> rounds.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th number in the list is the number of rounds the <span class="tex-span"><i>i</i></span>-th person wants to play.</p>

## Output

<p>In a single line print a single integer — the minimum number of game rounds the friends need to let the <span class="tex-span"><i>i</i></span>-th person play at least <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> rounds.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3
3 2 2

```




```input2
4
2 2 2 2

```




```output1
4

```




```output2
3

```



## Note

<p>You don't need to know the rules of "Mafia" to solve this problem. If you're curious, it's a game Russia got from the Soviet times: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Mafia_(party_game)</span>.</p>
