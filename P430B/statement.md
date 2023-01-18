## Description

<div><p>Iahub is training for the IOI. What is a better way to train than playing a Zuma-like game? </p><p>There are <span class="tex-span"><i>n</i></span> balls put in a row. Each ball is colored in one of <span class="tex-span"><i>k</i></span> colors. Initially the row doesn't contain three or more contiguous balls with the same color. Iahub has a single ball of color <span class="tex-span"><i>x</i></span>. He can insert his ball at any position in the row (probably, between two other balls). If at any moment there are three or more contiguous balls of the same color in the row, they are destroyed immediately. This rule is applied multiple times, until there are no more sets of 3 or more contiguous balls of the same color. </p><p>For example, if Iahub has the row of balls [black, black, white, white, black, black] and a white ball, he can insert the ball between two white balls. Thus three white balls are destroyed, and then four black balls become contiguous, so all four balls are destroyed. The row will not contain any ball in the end, so Iahub can destroy all 6 balls.</p><p>Iahub wants to destroy as many balls as possible. You are given the description of the row of balls, and the color of Iahub's ball. Help Iahub train for the IOI by telling him the maximum number of balls from the row he can destroy.</p></div><div class="input-specification"><p>The first line of input contains three integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>k</i></span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>). Number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> means that the <span class="tex-span"><i>i</i></span>-th ball in the row has color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the initial row of balls will never contain three or more contiguous balls of the same color. </p></div><div class="output-specification"><p>Print a single integer — the maximum number of balls Iahub can destroy.</p></div>

## Input

<p>The first line of input contains three integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>k</i></span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>). Number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> means that the <span class="tex-span"><i>i</i></span>-th ball in the row has color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the initial row of balls will never contain three or more contiguous balls of the same color. </p>

## Output

<p>Print a single integer — the maximum number of balls Iahub can destroy.</p>





```input1
6 2 2
1 1 2 2 1 1

```




```input2
1 1 1
1

```




```output1
6

```




```output2
0

```


