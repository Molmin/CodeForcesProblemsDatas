## Description

<div><p>You are given a sequence of numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, and a number <span class="tex-span"><i>m</i></span>.</p><p>Check if it is possible to choose a non-empty subsequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>j</i></sub></sub></span> such that the sum of numbers in this subsequence is divisible by <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first line contains two numbers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">3</sup></span>) — the size of the original sequence and the number such that sum should be divisible by it.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In the single line print either "<span class="tex-font-style-tt">YES</span>" (without the quotes) if there exists the sought subsequence, or "<span class="tex-font-style-tt">NO</span>" (without the quotes), if such subsequence doesn't exist.</p></div>

## Input

<p>The first line contains two numbers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">3</sup></span>) — the size of the original sequence and the number such that sum should be divisible by it.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In the single line print either "<span class="tex-font-style-tt">YES</span>" (without the quotes) if there exists the sought subsequence, or "<span class="tex-font-style-tt">NO</span>" (without the quotes), if such subsequence doesn't exist.</p>





```input1
3 5
1 2 3

```




```input2
1 6
5

```




```input3
4 6
3 1 1 3

```




```input4
6 6
5 5 5 5 5 5

```




```output1
YES

```




```output2
NO

```




```output3
YES

```




```output4
YES

```



## Note

<p>In the first sample test you can choose numbers <span class="tex-span">2</span> and <span class="tex-span">3</span>, the sum of which is divisible by <span class="tex-span">5</span>.</p><p>In the second sample test the single non-empty subsequence of numbers is a single number <span class="tex-span">5</span>. Number <span class="tex-span">5</span> is not divisible by <span class="tex-span">6</span>, that is, the sought subsequence doesn't exist.</p><p>In the third sample test you need to choose two numbers <span class="tex-span">3</span> on the ends.</p><p>In the fourth sample test you can take the whole subsequence.</p>
