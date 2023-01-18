## Description

<div><p>Recently, Duff has been practicing weight lifting. As a hard practice, Malek gave her a task. He gave her a sequence of weights. Weight of <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span">2<sup class="upper-index"><i>w</i><sub class="lower-index"><i>i</i></sub></sup></span> pounds. In each step, Duff can lift some of the remaining weights and throw them away. She does this until there's no more weight left. Malek asked her to minimize the number of steps.</p><center> <img class="tex-graphics" src="file://JqRhiey8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Duff is a competitive programming fan. That's why in each step, she can only lift and throw away a sequence of weights <span class="tex-span">2<sup class="upper-index"><i>a</i><sub class="lower-index">1</sub></sup>, ..., 2<sup class="upper-index"><i>a</i><sub class="lower-index"><i>k</i></sub></sup></span> if and only if there exists a non-negative integer <span class="tex-span"><i>x</i></span> such that <span class="tex-span">2<sup class="upper-index"><i>a</i><sub class="lower-index">1</sub></sup> + 2<sup class="upper-index"><i>a</i><sub class="lower-index">2</sub></sup> + ... + 2<sup class="upper-index"><i>a</i><sub class="lower-index"><i>k</i></sub></sup> = 2<sup class="upper-index"><i>x</i></sup></span>, i. e. the sum of those numbers is a power of two.</p><p>Duff is a competitive programming fan, but not a programmer. That's why she asked for your help. Help her minimize the number of steps. </p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>), the number of weights.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> separated by spaces (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), the powers of two forming the weights values.</p></div><div class="output-specification"><p>Print the minimum number of steps in a single line.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>), the number of weights.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> separated by spaces (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), the powers of two forming the weights values.</p>

## Output

<p>Print the minimum number of steps in a single line.</p>





```input1
5
1 1 2 3 3

```




```input2
4
0 1 2 3

```




```output1
2

```




```output2
4

```



## Note

<p>In the first sample case: One optimal way would be to throw away the first three in the first step and the rest in the second step. Also, it's not possible to do it in one step because their sum is not a power of two.</p><p>In the second sample case: The only optimal way is to throw away one weight in each step. It's not possible to do it in less than 4 steps because there's no subset of weights with more than one weight and sum equal to a power of two.</p>
