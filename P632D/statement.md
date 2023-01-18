## Description

<div><p>You are given array <span class="tex-span"><i>a</i></span> with <span class="tex-span"><i>n</i></span> elements and the number <span class="tex-span"><i>m</i></span>. Consider some subsequence of <span class="tex-span"><i>a</i></span> and the value of least common multiple (LCM) of its elements. Denote LCM as <span class="tex-span"><i>l</i></span>. Find any longest subsequence of <span class="tex-span"><i>a</i></span> with the value <span class="tex-span"><i>l</i> ≤ <i>m</i></span>.</p><p>A subsequence of <span class="tex-span"><i>a</i></span> is an array we can get by erasing some elements of <span class="tex-span"><i>a</i></span>. It is allowed to erase zero or all elements.</p><p>The LCM of an empty array equals <span class="tex-span">1</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the size of the array <span class="tex-span"><i>a</i></span> and the parameter from the problem statement.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>In the first line print two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>max</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>m</i>, 0 ≤ <i>k</i><sub class="lower-index"><i>max</i></sub> ≤ <i>n</i></span>) — the value of LCM and the number of elements in optimal subsequence.</p><p>In the second line print <span class="tex-span"><i>k</i><sub class="lower-index"><i>max</i></sub></span> integers — the positions of the elements from the optimal subsequence in the ascending order.</p><p>Note that you can find and print any subsequence with the maximum length.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the size of the array <span class="tex-span"><i>a</i></span> and the parameter from the problem statement.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>In the first line print two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>max</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>m</i>, 0 ≤ <i>k</i><sub class="lower-index"><i>max</i></sub> ≤ <i>n</i></span>) — the value of LCM and the number of elements in optimal subsequence.</p><p>In the second line print <span class="tex-span"><i>k</i><sub class="lower-index"><i>max</i></sub></span> integers — the positions of the elements from the optimal subsequence in the ascending order.</p><p>Note that you can find and print any subsequence with the maximum length.</p>





```input1
7 8
6 2 9 2 7 2 3

```




```input2
6 4
2 2 2 3 3 3

```




```output1
6 5
1 2 4 6 7

```




```output2
2 3
1 2 3

```


