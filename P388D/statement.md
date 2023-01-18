## Description

<div><p>Fox Ciel studies number theory.</p><p>She thinks a non-empty set <span class="tex-span"><i>S</i></span> contains non-negative integers is <span class="tex-font-style-it">perfect</span> if and only if for any <img align="middle" class="tex-formula" src="file://Be2Gmslw.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span"><i>a</i></span> can be equal to <span class="tex-span"><i>b</i></span>), <img align="middle" class="tex-formula" src="file://qKL3mLZd.png" style="max-width: 100.0%;max-height: 100.0%;">. Where operation <span class="tex-span"><i>xor</i></span> means exclusive or operation (<span class="tex-font-style-it">http://en.wikipedia.org/wiki/Exclusive_or</span>).</p><p>Please calculate the number of perfect sets consisting of integers not greater than <span class="tex-span"><i>k</i></span>. The answer can be very large, so print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print a single integer — the number of required sets modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print a single integer — the number of required sets modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1

```




```input2
2

```




```input3
3

```




```input4
4

```




```output1
2

```




```output2
3

```




```output3
5

```




```output4
6

```



## Note

<p>In example 1, there are 2 such sets: {0} and {0, 1}. Note that {1} is not a perfect set since 1 xor 1 = 0 and {1} doesn't contain zero.</p><p>In example 4, there are 6 such sets: {0}, {0, 1}, {0, 2}, {0, 3}, {0, 4} and {0, 1, 2, 3}.</p>
