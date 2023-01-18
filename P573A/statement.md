## Description

<div><p>Limak is an old brown bear. He often plays poker with his friends. Today they went to a casino. There are <span class="tex-span"><i>n</i></span> players (including Limak himself) and right now all of them have bids on the table. <span class="tex-span"><i>i</i></span>-th of them has bid with size <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> dollars.</p><p>Each player can double his bid any number of times and triple his bid any number of times. The casino has a great jackpot for making all bids equal. Is it possible that Limak and his friends will win a jackpot?</p></div><div class="input-specification"><p>First line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of players.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the bids of players.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" (without the quotes) if players can make their bids become equal, or "<span class="tex-font-style-tt">No</span>" otherwise.</p></div>

## Input

<p>First line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of players.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the bids of players.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" (without the quotes) if players can make their bids become equal, or "<span class="tex-font-style-tt">No</span>" otherwise.</p>





```input1
4
75 150 75 50

```




```input2
3
100 150 250

```




```output1
Yes

```




```output2
No

```



## Note

<p>In the first sample test first and third players should double their bids twice, second player should double his bid once and fourth player should both double and triple his bid.</p><p>It can be shown that in the second sample test there is no way to make all bids equal.</p>
