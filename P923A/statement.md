## Description

<div><p>Alice and Bob begin their day with a quick game. They first choose a starting number <span class="tex-span"><i>X</i><sub class="lower-index">0</sub> ≥ 3</span> and try to reach one million by the process described below. </p><p>Alice goes first and then they take alternating turns. In the <span class="tex-span"><i>i</i></span>-th turn, the player whose turn it is selects a prime number smaller than the current number, and announces the smallest multiple of this prime number that is not smaller than the current number.</p><p>Formally, he or she selects a prime <span class="tex-span"><i>p</i> &lt; <i>X</i><sub class="lower-index"><i>i</i> - 1</sub></span> and then finds the minimum <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub> ≥ <i>X</i><sub class="lower-index"><i>i</i> - 1</sub></span> such that <span class="tex-span"><i>p</i></span> divides <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub></span>. Note that if the selected prime <span class="tex-span"><i>p</i></span> already divides <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i> - 1</sub></span>, then the number does not change.</p><p>Eve has witnessed the state of the game after two turns. Given <span class="tex-span"><i>X</i><sub class="lower-index">2</sub></span>, help her determine what is the smallest possible starting number <span class="tex-span"><i>X</i><sub class="lower-index">0</sub></span>. Note that the players don't necessarily play optimally. You should consider all possible game evolutions.</p></div><div class="input-specification"><p>The input contains a single integer <span class="tex-span"><i>X</i><sub class="lower-index">2</sub></span> (<span class="tex-span">4 ≤ <i>X</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>). It is guaranteed that the integer <span class="tex-span"><i>X</i><sub class="lower-index">2</sub></span> is composite, that is, is not prime.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the minimum possible <span class="tex-span"><i>X</i><sub class="lower-index">0</sub></span>.</p></div>

## Input

<p>The input contains a single integer <span class="tex-span"><i>X</i><sub class="lower-index">2</sub></span> (<span class="tex-span">4 ≤ <i>X</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>). It is guaranteed that the integer <span class="tex-span"><i>X</i><sub class="lower-index">2</sub></span> is composite, that is, is not prime.</p>

## Output

<p>Output a single integer&nbsp;— the minimum possible <span class="tex-span"><i>X</i><sub class="lower-index">0</sub></span>.</p>





```input1
14

```




```input2
20

```




```input3
8192

```




```output1
6

```




```output2
15

```




```output3
8191

```



## Note

<p>In the first test, the smallest possible starting number is <span class="tex-span"><i>X</i><sub class="lower-index">0</sub> = 6</span>. One possible course of the game is as follows: </p><ul> <li> Alice picks prime 5 and announces <span class="tex-span"><i>X</i><sub class="lower-index">1</sub> = 10</span> </li><li> Bob picks prime 7 and announces <span class="tex-span"><i>X</i><sub class="lower-index">2</sub> = 14</span>. </li></ul><p>In the second case, let <span class="tex-span"><i>X</i><sub class="lower-index">0</sub> = 15</span>. </p><ul> <li> Alice picks prime 2 and announces <span class="tex-span"><i>X</i><sub class="lower-index">1</sub> = 16</span> </li><li> Bob picks prime 5 and announces <span class="tex-span"><i>X</i><sub class="lower-index">2</sub> = 20</span>. </li></ul>
