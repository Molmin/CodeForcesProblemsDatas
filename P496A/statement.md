## Description

<div><p>Mike is trying rock climbing but he is awful at it. </p><p>There are <span class="tex-span"><i>n</i></span> holds on the wall, <span class="tex-span"><i>i</i></span>-th hold is at height <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> off the ground. Besides, let the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> increase, that is, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>n</i> - 1</span>; we will call such sequence a <span class="tex-font-style-underline">track</span>. Mike thinks that the track <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> has <span class="tex-font-style-underline">difficulty</span> <img align="middle" class="tex-formula" src="file://2VgfRC7l.png" style="max-width: 100.0%;max-height: 100.0%;">. In other words, difficulty equals the maximum distance between two holds that are adjacent in height.</p><p>Today Mike decided to cover the track with holds hanging on heights <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. To make the problem harder, Mike decided to remove one hold, that is, remove one element of the sequence (for example, if we take the sequence <span class="tex-span">(1, 2, 3, 4, 5)</span> and remove the third element from it, we obtain the sequence <span class="tex-span">(1, 2, 4, 5)</span>). However, as Mike is awful at climbing, he wants the final difficulty (i.e. the maximum difference of heights between adjacent holds after removing the hold) to be as small as possible among all possible options of removing a hold. The first and last holds <span class="tex-font-style-bf">must</span> stay at their positions.</p><p>Help Mike determine the minimum difficulty of the track after removing one hold.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of holds.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the height where the hold number <span class="tex-span"><i>i</i></span> hangs. The sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is increasing (i.e. each element except for the first one is strictly larger than the previous one).</p></div><div class="output-specification"><p>Print a single number — the minimum difficulty of the track after removing a single hold.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of holds.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the height where the hold number <span class="tex-span"><i>i</i></span> hangs. The sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is increasing (i.e. each element except for the first one is strictly larger than the previous one).</p>

## Output

<p>Print a single number — the minimum difficulty of the track after removing a single hold.</p>





```input1
3
1 4 6

```




```input2
5
1 2 3 4 5

```




```input3
5
1 2 3 7 8

```




```output1
5

```




```output2
2

```




```output3
4

```



## Note

<p>In the first sample you can remove only the second hold, then the sequence looks like <span class="tex-span">(1, 6)</span>, the maximum difference of the neighboring elements equals 5.</p><p>In the second test after removing every hold the difficulty equals 2.</p><p>In the third test you can obtain sequences <span class="tex-span">(1, 3, 7, 8)</span>, <span class="tex-span">(1, 2, 7, 8)</span>, <span class="tex-span">(1, 2, 3, 8)</span>, for which the difficulty is 4, 5 and 5, respectively. Thus, after removing the second element we obtain the optimal answer — 4.</p>
