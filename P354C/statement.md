## Description

<div><p>Vasya's got a birthday coming up and his mom decided to give him an array of positive integers <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span>.</p><p>Vasya thinks that an array's beauty is the greatest common divisor of all its elements. His mom, of course, wants to give him as beautiful an array as possible (with largest possible beauty). Unfortunately, the shop has only one array <span class="tex-span"><i>a</i></span> left. On the plus side, the seller said that he could decrease some numbers in the array (no more than by <span class="tex-span"><i>k</i></span> for each number).</p><p>The seller can obtain array <span class="tex-span"><i>b</i></span> from array <span class="tex-span"><i>a</i></span> if the following conditions hold: <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &gt; 0; 0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> - <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span> for all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>.</p><p>Help mom find the maximum possible beauty of the array she will give to Vasya (that seller can obtain).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>; 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>In the single line print a single number — the maximum possible beauty of the resulting array.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>; 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>In the single line print a single number — the maximum possible beauty of the resulting array.</p>





```input1
6 1
3 6 10 12 13 16

```




```input2
5 3
8 21 52 15 77

```




```output1
3

```




```output2
7

```



## Note

<p>In the first sample we can obtain the array:</p><p><span class="tex-span">3 6 9 12 12 15</span></p><p>In the second sample we can obtain the next array:</p><p><span class="tex-span">7 21 49 14 77</span></p>
