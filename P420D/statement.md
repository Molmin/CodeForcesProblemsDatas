## Description

<div><p>The employees of the F company have lots of ways to entertain themselves. Today they invited a famous magician who shows a trick with plastic cups and a marble.</p><p>The point is to trick the spectator's attention. Initially, the spectator stands in front of a line of <span class="tex-span"><i>n</i></span> plastic cups. Then the magician places a small marble under one cup and shuffles the cups. Then the spectator should guess which cup hides the marble.</p><p>But the head coder of the F company isn't easy to trick. When he saw the performance, he noticed several important facts:</p><ul> <li> each cup contains a mark — a number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>; all marks on the cups are distinct; </li><li> the magician shuffles the cups in <span class="tex-span"><i>m</i></span> operations, each operation looks like that: take a cup marked <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, sitting at position <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> in the row of cups (the positions are numbered from left to right, starting from 1) and shift it to the very beginning of the cup row (on the first position). </li></ul><p>When the head coder came home after work he wanted to re-do the trick. Unfortunately, he didn't remember the starting or the final position of the cups. He only remembered which operations the magician performed. Help the coder: given the operations in the order they were made find at least one initial permutation of the cups that can go through the described operations in the given order. Otherwise, state that such permutation doesn't exist.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains a couple of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the description of the <span class="tex-span"><i>i</i></span>-th operation of the magician. Note that the operations are given in the order in which the magician made them and the coder wants to make them in the same order.</p></div><div class="output-specification"><p>If the described permutation doesn't exist (the programmer remembered wrong operations), print -1. Otherwise, print <span class="tex-span"><i>n</i></span> distinct integers, each from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>: the <span class="tex-span"><i>i</i></span>-th number should represent the mark on the cup that initially is in the row in position <span class="tex-span"><i>i</i></span>.</p><p>If there are multiple correct answers, you should print the lexicographically minimum one.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains a couple of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the description of the <span class="tex-span"><i>i</i></span>-th operation of the magician. Note that the operations are given in the order in which the magician made them and the coder wants to make them in the same order.</p>

## Output

<p>If the described permutation doesn't exist (the programmer remembered wrong operations), print -1. Otherwise, print <span class="tex-span"><i>n</i></span> distinct integers, each from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>: the <span class="tex-span"><i>i</i></span>-th number should represent the mark on the cup that initially is in the row in position <span class="tex-span"><i>i</i></span>.</p><p>If there are multiple correct answers, you should print the lexicographically minimum one.</p>





```input1
2 1
2 1

```




```input2
3 2
1 2
1 1

```




```input3
3 3
1 3
2 3
1 3

```




```output1
2 1 

```




```output2
2 1 3 

```




```output3
-1

```


