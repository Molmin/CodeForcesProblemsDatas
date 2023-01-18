## Description

<div><p><span class="tex-font-style-it"> — Oh my sweet Beaverette, would you fancy a walk along a wonderful woodland belt with me? </span> </p><p><span class="tex-font-style-it"> — Of course, my Smart Beaver! Let us enjoy the splendid view together. How about Friday night? </span></p><p>At this point the Smart Beaver got rushing. Everything should be perfect by Friday, so he needed to prepare the belt to the upcoming walk. He needed to cut down several trees.</p><p>Let's consider the woodland belt as a sequence of trees. Each tree <span class="tex-span"><i>i</i></span> is described by the esthetic appeal <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — some trees are very esthetically pleasing, others are 'so-so', and some trees are positively ugly!</p><p>The Smart Beaver calculated that he needed the following effects to win the Beaverette's heart: </p><ul> <li> The first objective is to please the Beaverette: the sum of esthetic appeal of the remaining trees must be maximum possible; </li><li> the second objective is to surprise the Beaverette: the esthetic appeal of the first and the last trees in the resulting belt must be the same; </li><li> and of course, the walk should be successful: there must be at least two trees in the woodland belt left. </li></ul><p>Now help the Smart Beaver! Which trees does he need to cut down to win the Beaverette's heart?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> — the initial number of trees in the woodland belt, <span class="tex-span">2 ≤ <i>n</i></span>. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the esthetic appeals of each tree. All esthetic appeals do not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> in their absolute value.</p><ul> <li> to get 30 points, you need to solve the problem with constraints: <span class="tex-span"><i>n</i> ≤ 100</span> (subproblem A1); </li><li> to get 100 points, you need to solve the problem with constraints: <span class="tex-span"><i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span> (subproblems A1+A2). </li></ul></div><div class="output-specification"><p>In the first line print two integers — the total esthetic appeal of the woodland belt after the Smart Beaver's intervention and the number of the cut down trees <span class="tex-span"><i>k</i></span>.</p><p>In the next line print <span class="tex-span"><i>k</i></span> integers — the numbers of the trees the Beaver needs to cut down. Assume that the trees are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right.</p><p>If there are multiple solutions, print any of them. It is guaranteed that at least two trees have equal esthetic appeal.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> — the initial number of trees in the woodland belt, <span class="tex-span">2 ≤ <i>n</i></span>. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the esthetic appeals of each tree. All esthetic appeals do not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> in their absolute value.</p><ul> <li> to get 30 points, you need to solve the problem with constraints: <span class="tex-span"><i>n</i> ≤ 100</span> (subproblem A1); </li><li> to get 100 points, you need to solve the problem with constraints: <span class="tex-span"><i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span> (subproblems A1+A2). </li></ul>

## Output

<p>In the first line print two integers — the total esthetic appeal of the woodland belt after the Smart Beaver's intervention and the number of the cut down trees <span class="tex-span"><i>k</i></span>.</p><p>In the next line print <span class="tex-span"><i>k</i></span> integers — the numbers of the trees the Beaver needs to cut down. Assume that the trees are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right.</p><p>If there are multiple solutions, print any of them. It is guaranteed that at least two trees have equal esthetic appeal.</p>





```input1
5
1 2 3 1 2

```




```input2
5
1 -2 3 1 -2

```




```output1
8 1
1
```




```output2
5 2
2 5
```


