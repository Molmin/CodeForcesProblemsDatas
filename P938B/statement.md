## Description

<div><p>You and your friend are participating in a TV show "Run For Your Prize".</p><p>At the start of the show <span class="tex-span"><i>n</i></span> prizes are located on a straight line. <span class="tex-span"><i>i</i></span>-th prize is located at position <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Positions of all prizes are distinct. You start at position <span class="tex-span">1</span>, your friend — at position <span class="tex-span">10<sup class="upper-index">6</sup></span> (and there is no prize in any of these two positions). You have to work as a team and collect all prizes in minimum possible time, in any order.</p><p>You know that it takes exactly <span class="tex-span">1</span> second to move from position <span class="tex-span"><i>x</i></span> to position <span class="tex-span"><i>x</i> + 1</span> or <span class="tex-span"><i>x</i> - 1</span>, both for you and your friend. You also have trained enough to instantly pick up any prize, if its position is equal to your current position (and the same is true for your friend). Carrying prizes does not affect your speed (or your friend's speed) at all.</p><p>Now you may discuss your strategy with your friend and decide who will pick up each prize. Remember that every prize must be picked up, either by you or by your friend.</p><p>What is the minimum number of seconds it will take to pick up all the prizes?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of prizes.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup> - 1</span>) — the positions of the prizes. No two prizes are located at the same position. Positions are given in ascending order.</p></div><div class="output-specification"><p>Print one integer — the minimum number of seconds it will take to collect all prizes.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of prizes.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup> - 1</span>) — the positions of the prizes. No two prizes are located at the same position. Positions are given in ascending order.</p>

## Output

<p>Print one integer — the minimum number of seconds it will take to collect all prizes.</p>





```input1
3
2 3 9

```




```input2
2
2 999995

```




```output1
8

```




```output2
5

```



## Note

<p>In the first example you take all the prizes: take the first at <span class="tex-span">1</span>, the second at <span class="tex-span">2</span> and the third at <span class="tex-span">8</span>.</p><p>In the second example you take the first prize in <span class="tex-span">1</span> second and your friend takes the other in <span class="tex-span">5</span> seconds, you do this simultaneously, so the total time is <span class="tex-span">5</span>.</p>
