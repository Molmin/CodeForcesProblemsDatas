## Description

<div><p>There is a game called "I Wanna Be the Guy", consisting of <span class="tex-span"><i>n</i></span> levels. Little X and his friend Little Y are addicted to the game. Each of them wants to pass the whole game.</p><p>Little X can pass only <span class="tex-span"><i>p</i></span> levels of the game. And Little Y can pass only <span class="tex-span"><i>q</i></span> levels of the game. You are given the indices of levels Little X can pass and the indices of levels Little Y can pass. Will Little X and Little Y pass the whole game, if they cooperate each other?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤  <i>n</i> ≤ 100</span>). </p><p>The next line contains an integer <span class="tex-span"><i>p</i></span> <span class="tex-span">(0 ≤ <i>p</i> ≤ <i>n</i>)</span> at first, then follows <span class="tex-span"><i>p</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>p</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. These integers denote the indices of levels Little X can pass. The next line contains the levels Little Y can pass in the same format. It's assumed that levels are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>If they can pass all the levels, print "<span class="tex-font-style-tt">I become the guy.</span>". If it's impossible, print "<span class="tex-font-style-tt">Oh, my keyboard!</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤  <i>n</i> ≤ 100</span>). </p><p>The next line contains an integer <span class="tex-span"><i>p</i></span> <span class="tex-span">(0 ≤ <i>p</i> ≤ <i>n</i>)</span> at first, then follows <span class="tex-span"><i>p</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>p</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. These integers denote the indices of levels Little X can pass. The next line contains the levels Little Y can pass in the same format. It's assumed that levels are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>If they can pass all the levels, print "<span class="tex-font-style-tt">I become the guy.</span>". If it's impossible, print "<span class="tex-font-style-tt">Oh, my keyboard!</span>" (without the quotes).</p>





```input1
4
3 1 2 3
2 2 4

```




```input2
4
3 1 2 3
2 2 3

```




```output1
I become the guy.

```




```output2
Oh, my keyboard!

```



## Note

<p>In the first sample, Little X can pass levels [1 2 3], and Little Y can pass level [2 4], so they can pass all the levels both.</p><p>In the second sample, no one can pass level 4.</p>
