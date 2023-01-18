## Description

<div><p>Mahmoud has an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers. He asked Ehab to find another array <span class="tex-span"><i>b</i></span> <span class="tex-font-style-bf">of the same length</span> such that:</p><ul> <li> <span class="tex-span"><i>b</i></span> is lexicographically greater than or equal to <span class="tex-span"><i>a</i></span>. </li><li> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≥ 2</span>. </li><li> <span class="tex-span"><i>b</i></span> is pairwise coprime: for every <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> are coprime, i.&nbsp;e. <span class="tex-span"><i>GCD</i>(<i>b</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>) = 1</span>, where <span class="tex-span"><i>GCD</i>(<i>w</i>, <i>z</i>)</span> is the greatest common divisor of <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>z</i></span>. </li></ul><p>Ehab wants to choose a special array so he wants the lexicographically minimal array between all the variants. Can you find it?</p><p>An array <span class="tex-span"><i>x</i></span> is lexicographically greater than an array <span class="tex-span"><i>y</i></span> if there exists an index <span class="tex-span"><i>i</i></span> such than <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &gt; <i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span> for all <span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>. An array <span class="tex-span"><i>x</i></span> is equal to an array <span class="tex-span"><i>y</i></span> if <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of elements in <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, the elements of <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> space-separated integers, the <span class="tex-span"><i>i</i></span>-th of them representing <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of elements in <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, the elements of <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> space-separated integers, the <span class="tex-span"><i>i</i></span>-th of them representing <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
5
2 3 5 4 13

```




```input2
3
10 3 7

```




```output1
2 3 5 7 11
```




```output2
10 3 7
```



## Note

<p>Note that in the second sample, the array is already pairwise coprime so we printed it.</p>
