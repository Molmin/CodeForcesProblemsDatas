## Description

<div><p>Dima and Anya love playing different games. Now Dima has imagined a new game that he wants to play with Anya.</p><p>Dima writes <span class="tex-span"><i>n</i></span> pairs of integers on a piece of paper <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>p</i>)</span>. Then players take turns. On his turn the player can do the following actions:</p><ol> <li> choose the number of the pair <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span>, such that <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> - <i>l</i><sub class="lower-index"><i>i</i></sub> &gt; 2</span>; </li><li> replace pair number <span class="tex-span"><i>i</i></span> by pair <img align="middle" class="tex-formula" src="file://XwSG2AP5.png" style="max-width: 100.0%;max-height: 100.0%;"> or by pair <img align="middle" class="tex-formula" src="file://RZXVe92G.png" style="max-width: 100.0%;max-height: 100.0%;">. Notation <span class="tex-span">⌊<i>x</i>⌋</span> means rounding down to the closest integer. </li></ol><p>The player who can't make a move loses.</p><p>Of course, Dima wants Anya, who will move first, to win. That's why Dima should write out such <span class="tex-span"><i>n</i></span> pairs of integers <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>p</i>)</span>, that if both players play optimally well, the first one wins. Count the number of ways in which Dima can do it. Print the remainder after dividing the answer by number <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p><p>Two ways are considered distinct, if the <span class="tex-font-style-bf">ordered</span> sequences of the written pairs are distinct.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The numbers are separated by a single space.</p></div><div class="output-specification"><p>In a single line print the remainder after dividing the answer to the problem by number <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The numbers are separated by a single space.</p>

## Output

<p>In a single line print the remainder after dividing the answer to the problem by number <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2 2

```




```input2
4 4

```




```input3
100 1000

```




```output1
0

```




```output2
520

```




```output3
269568947

```


