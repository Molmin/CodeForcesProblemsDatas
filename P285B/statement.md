## Description

<div><p>Petya and Vasya are playing a game. Petya's got <span class="tex-span"><i>n</i></span> non-transparent glasses, standing in a row. The glasses' positions are indexed with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Note that the positions are indexed but the glasses are not.</p><p>First Petya puts a marble under the glass in position <span class="tex-span"><i>s</i></span>. Then he performs some (possibly zero) shuffling operations. One shuffling operation means moving the glass from the first position to position <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, the glass from the second position to position <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> and so on. That is, a glass goes from position <span class="tex-span"><i>i</i></span> to position <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Consider all glasses are moving simultaneously during one shuffling operation. When the glasses are shuffled, the marble doesn't travel from one glass to another: it moves together with the glass it was initially been put in.</p><p>After all shuffling operations Petya shows Vasya that the ball has moved to position <span class="tex-span"><i>t</i></span>. Vasya's task is to say what minimum number of shuffling operations Petya has performed or determine that Petya has made a mistake and the marble could not have got from position <span class="tex-span"><i>s</i></span> to position <span class="tex-span"><i>t</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers: <span class="tex-span"><i>n</i>, <i>s</i>, <i>t</i> (1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i>)</span> — the number of glasses, the ball's initial and final position. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub> (1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the shuffling operation parameters. It is guaranteed that all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct.</p><p>Note that <span class="tex-span"><i>s</i></span> can equal <span class="tex-span"><i>t</i></span>.</p></div><div class="output-specification"><p>If the marble can move from position <span class="tex-span"><i>s</i></span> to position <span class="tex-span"><i>t</i></span>, then print on a single line a non-negative integer — the minimum number of shuffling operations, needed to get the marble to position <span class="tex-span"><i>t</i></span>. If it is impossible, print number -1.</p></div>

## Input

<p>The first line contains three integers: <span class="tex-span"><i>n</i>, <i>s</i>, <i>t</i> (1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i>)</span> — the number of glasses, the ball's initial and final position. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub> (1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the shuffling operation parameters. It is guaranteed that all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct.</p><p>Note that <span class="tex-span"><i>s</i></span> can equal <span class="tex-span"><i>t</i></span>.</p>

## Output

<p>If the marble can move from position <span class="tex-span"><i>s</i></span> to position <span class="tex-span"><i>t</i></span>, then print on a single line a non-negative integer — the minimum number of shuffling operations, needed to get the marble to position <span class="tex-span"><i>t</i></span>. If it is impossible, print number -1.</p>





```input1
4 2 1
2 3 4 1

```




```input2
4 3 3
4 1 3 2

```




```input3
4 3 4
1 2 3 4

```




```input4
3 1 3
2 1 3

```




```output1
3

```




```output2
0

```




```output3
-1

```




```output4
-1

```


