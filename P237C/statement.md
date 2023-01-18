## Description

<div><p>You've decided to carry out a survey in the theory of prime numbers. Let us remind you that a prime number is a positive integer that has exactly two distinct positive integer divisors.</p><p>Consider positive integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>a</i> + 1</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>a</i> ≤ <i>b</i>)</span>. You want to find the minimum integer <span class="tex-span"><i>l</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>b</i> - <i>a</i> + 1)</span> such that for any integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>a</i> ≤ <i>x</i> ≤ <i>b</i> - <i>l</i> + 1)</span> among <span class="tex-span"><i>l</i></span> integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>x</i> + 1</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>x</i> + <i>l</i> - 1</span> there are at least <span class="tex-span"><i>k</i></span> prime numbers. </p><p>Find and print the required minimum <span class="tex-span"><i>l</i></span>. If no value <span class="tex-span"><i>l</i></span> meets the described limitations, print -1.</p></div><div class="input-specification"><p>A single line contains three space-separated integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>k</i> ≤ 10<sup class="upper-index">6</sup>;&nbsp;<i>a</i> ≤ <i>b</i></span>).</p></div><div class="output-specification"><p>In a single line print a single integer — the required minimum <span class="tex-span"><i>l</i></span>. If there's no solution, print -1.</p></div>

## Input

<p>A single line contains three space-separated integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>k</i> ≤ 10<sup class="upper-index">6</sup>;&nbsp;<i>a</i> ≤ <i>b</i></span>).</p>

## Output

<p>In a single line print a single integer — the required minimum <span class="tex-span"><i>l</i></span>. If there's no solution, print -1.</p>





```input1
2 4 2

```




```input2
6 13 1

```




```input3
1 4 3

```




```output1
3

```




```output2
4

```




```output3
-1

```


