## Description

<div><p>It's holiday. Mashmokh and his boss, Bimokh, are playing a game invented by Mashmokh. </p><p>In this game Mashmokh writes sequence of <span class="tex-span"><i>n</i></span> distinct integers on the board. Then Bimokh makes several (possibly zero) moves. On the first move he removes the first and the second integer from from the board, on the second move he removes the first and the second integer of the remaining sequence from the board, and so on. Bimokh stops when the board contains less than two numbers. When Bimokh removes numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> from the board, he gets <span class="tex-span"><i>gcd</i>(<i>x</i>, <i>y</i>)</span> points. At the beginning of the game Bimokh has zero points.</p><p>Mashmokh wants to win in the game. For this reason he wants his boss to get exactly <span class="tex-span"><i>k</i></span> points in total. But the guy doesn't know how choose the initial sequence in the right way. </p><p>Please, help him. Find <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> such that his boss will score exactly <span class="tex-span"><i>k</i></span> points. Also Mashmokh can't memorize too huge numbers. Therefore each of these integers must be at most <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>k</i> ≤ 10<sup class="upper-index">8</sup>)</span>.</p></div><div class="output-specification"><p>If such sequence doesn't exist output -1 otherwise output <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>k</i> ≤ 10<sup class="upper-index">8</sup>)</span>.</p>

## Output

<p>If such sequence doesn't exist output -1 otherwise output <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>





```input1
5 2

```




```input2
5 3
```




```input3
7 2

```




```output1
1 2 3 4 5

```




```output2
2 4 3 7 1
```




```output3
-1

```



## Note

<p><span class="tex-span"><i>gcd</i>(<i>x</i>, <i>y</i>)</span> is greatest common divisor of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p>
