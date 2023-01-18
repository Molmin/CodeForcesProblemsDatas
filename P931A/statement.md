## Description

<div><p>Two friends are on the coordinate axis <span class="tex-span"><i>Ox</i></span> in points with integer coordinates. One of them is in the point <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>a</i></span>, another one is in the point <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> = <i>b</i></span>. </p><p>Each of the friends can move by one along the line in any direction unlimited number of times. When a friend moves, the tiredness of a friend changes according to the following rules: the first move increases the tiredness by <span class="tex-span">1</span>, the second move increases the tiredness by <span class="tex-span">2</span>, the third&nbsp;— by <span class="tex-span">3</span> and so on. For example, if a friend moves first to the left, then to the right (returning to the same point), and then again to the left his tiredness becomes equal to <span class="tex-span">1 + 2 + 3 = 6</span>.</p><p>The friends want to meet in a integer point. Determine the minimum total tiredness they should gain, if they meet in the same point.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 1000</span>) — the initial position of the first friend. </p><p>The second line contains a single integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 1000</span>) — the initial position of the second friend.</p><p>It is guaranteed that <span class="tex-span"><i>a</i> ≠ <i>b</i></span>.</p></div><div class="output-specification"><p>Print the minimum possible total tiredness if the friends meet in the same point.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 1000</span>) — the initial position of the first friend. </p><p>The second line contains a single integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 1000</span>) — the initial position of the second friend.</p><p>It is guaranteed that <span class="tex-span"><i>a</i> ≠ <i>b</i></span>.</p>

## Output

<p>Print the minimum possible total tiredness if the friends meet in the same point.</p>





```input1
3
4

```




```input2
101
99

```




```input3
5
10

```




```output1
1

```




```output2
2

```




```output3
9

```



## Note

<p>In the first example the first friend should move by one to the right (then the meeting happens at point <span class="tex-span">4</span>), or the second friend should move by one to the left (then the meeting happens at point <span class="tex-span">3</span>). In both cases, the total tiredness becomes <span class="tex-span">1</span>.</p><p>In the second example the first friend should move by one to the left, and the second friend should move by one to the right. Then they meet in the point <span class="tex-span">100</span>, and the total tiredness becomes <span class="tex-span">1 + 1 = 2</span>.</p><p>In the third example one of the optimal ways is the following. The first friend should move three times to the right, and the second friend — two times to the left. Thus the friends meet in the point <span class="tex-span">8</span>, and the total tiredness becomes <span class="tex-span">1 + 2 + 3 + 1 + 2 = 9</span>.</p>
