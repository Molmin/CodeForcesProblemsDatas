## Description

<div><p>Alice and Bob like games. And now they are ready to start a new game. They have placed <span class="tex-span"><i>n</i></span> chocolate bars in a line. Alice starts to eat chocolate bars one by one from left to right, and Bob — from right to left. For each chocololate bar the time, needed for the player to consume it, is known (Alice and Bob eat them with equal speed). When the player consumes a chocolate bar, he immediately starts with another. It is not allowed to eat two chocolate bars at the same time, to leave the bar unfinished and to make pauses. If both players start to eat the same bar simultaneously, Bob leaves it to Alice as a true gentleman.</p><p>How many bars each of the players will consume?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the amount of bars on the table. The second line contains a sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the time (in seconds) needed to consume the <span class="tex-span"><i>i</i></span>-th bar (in the order from left to right).</p></div><div class="output-specification"><p>Print two numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, where <span class="tex-span"><i>a</i></span> is the amount of bars consumed by Alice, and <span class="tex-span"><i>b</i></span> is the amount of bars consumed by Bob.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the amount of bars on the table. The second line contains a sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the time (in seconds) needed to consume the <span class="tex-span"><i>i</i></span>-th bar (in the order from left to right).</p>

## Output

<p>Print two numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, where <span class="tex-span"><i>a</i></span> is the amount of bars consumed by Alice, and <span class="tex-span"><i>b</i></span> is the amount of bars consumed by Bob.</p>





```input1
5
2 9 8 2 7

```




```output1
2 3

```


