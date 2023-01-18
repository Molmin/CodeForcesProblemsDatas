## Description

<div><p>Petya and Vasya are tossing a coin. Their friend Valera is appointed as a judge. The game is very simple. First Vasya tosses a coin <span class="tex-span"><i>x</i></span> times, then Petya tosses a coin <span class="tex-span"><i>y</i></span> times. If the tossing player gets head, he scores one point. If he gets tail, nobody gets any points. The winner is the player with most points by the end of the game. If boys have the same number of points, the game finishes with a draw.</p><p>At some point, Valera lost his count, and so he can not say exactly what the score is at the end of the game. But there are things he remembers for sure. He remembers that the entire game Vasya got heads at least <span class="tex-span"><i>a</i></span> times, and Petya got heads at least <span class="tex-span"><i>b</i></span> times. Moreover, he knows that the winner of the game was Vasya. Valera wants to use this information to know every possible outcome of the game, which do not contradict his memories.</p></div><div class="input-specification"><p>The single line contains four integers <span class="tex-span"><i>x</i>, <i>y</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>x</i> ≤ 100, 1 ≤ <i>b</i> ≤ <i>y</i> ≤ 100)</span>. The numbers on the line are separated by a space.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>n</i></span> — the number of possible outcomes of the game. Then on <span class="tex-span"><i>n</i></span> lines print the outcomes. On the <span class="tex-span"><i>i</i></span>-th line print a space-separated pair of integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> — the number of heads Vasya and Petya got in the <span class="tex-span"><i>i</i></span>-th outcome of the game, correspondingly. Print pairs of integers <span class="tex-span">(<i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>)</span> in the strictly increasing order.</p><p>Let us remind you that the pair of numbers <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">1</sub>)</span> is less than the pair of numbers <span class="tex-span">(<i>p</i><sub class="lower-index">2</sub>, <i>q</i><sub class="lower-index">2</sub>)</span>, if <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub></span>, or <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = <i>p</i><sub class="lower-index">2</sub></span> and also <span class="tex-span"><i>q</i><sub class="lower-index">1</sub> &lt; <i>q</i><sub class="lower-index">2</sub></span>.</p></div>

## Input

<p>The single line contains four integers <span class="tex-span"><i>x</i>, <i>y</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>x</i> ≤ 100, 1 ≤ <i>b</i> ≤ <i>y</i> ≤ 100)</span>. The numbers on the line are separated by a space.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>n</i></span> — the number of possible outcomes of the game. Then on <span class="tex-span"><i>n</i></span> lines print the outcomes. On the <span class="tex-span"><i>i</i></span>-th line print a space-separated pair of integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> — the number of heads Vasya and Petya got in the <span class="tex-span"><i>i</i></span>-th outcome of the game, correspondingly. Print pairs of integers <span class="tex-span">(<i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>)</span> in the strictly increasing order.</p><p>Let us remind you that the pair of numbers <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">1</sub>)</span> is less than the pair of numbers <span class="tex-span">(<i>p</i><sub class="lower-index">2</sub>, <i>q</i><sub class="lower-index">2</sub>)</span>, if <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub></span>, or <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = <i>p</i><sub class="lower-index">2</sub></span> and also <span class="tex-span"><i>q</i><sub class="lower-index">1</sub> &lt; <i>q</i><sub class="lower-index">2</sub></span>.</p>





```input1
3 2 1 1

```




```input2
2 4 2 2

```




```output1
3
2 1
3 1
3 2

```




```output2
0

```


