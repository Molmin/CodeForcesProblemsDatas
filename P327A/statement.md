## Description

<div><p>Iahub got bored, so he invented a game to be played on paper. </p><p>He writes <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Each of those integers can be either 0 or 1. He's allowed to do exactly one move: he chooses two indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span>) and flips all values <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> for which their positions are in range <span class="tex-span">[<i>i</i>, <i>j</i>]</span> (that is <span class="tex-span"><i>i</i> ≤ <i>k</i> ≤ <i>j</i></span>). Flip the value of <span class="tex-span"><i>x</i></span> means to apply operation <span class="tex-span"><i>x</i> = 1</span> - <span class="tex-span"><i>x</i></span>.</p><p>The goal of the game is that after <span class="tex-font-style-bf">exactly</span> one move to obtain the maximum number of ones. Write a program to solve the little game of Iahub.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). In the second line of the input there are <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. It is guaranteed that each of those <span class="tex-span"><i>n</i></span> values is either 0 or 1.</p></div><div class="output-specification"><p>Print an integer — the maximal number of 1s that can be obtained after exactly one move. </p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). In the second line of the input there are <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. It is guaranteed that each of those <span class="tex-span"><i>n</i></span> values is either 0 or 1.</p>

## Output

<p>Print an integer — the maximal number of 1s that can be obtained after exactly one move. </p>





```input1
5
1 0 0 1 0

```




```input2
4
1 0 0 1

```




```output1
4

```




```output2
4

```



## Note

<p>In the first case, flip the segment from 2 to 5 <span class="tex-span">(<i>i</i> = 2, <i>j</i> = 5)</span>. That flip changes the sequence, it becomes: [1 1 1 0 1]. So, it contains four ones. There is no way to make the whole sequence equal to [1 1 1 1 1].</p><p>In the second case, flipping only the second and the third element <span class="tex-span">(<i>i</i> = 2, <i>j</i> = 3)</span> will turn all numbers into 1.</p>
