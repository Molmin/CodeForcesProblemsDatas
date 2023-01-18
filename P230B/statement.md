## Description

<div><p>We know that prime numbers are positive integers that have exactly two distinct positive divisors. Similarly, we'll call a positive integer <span class="tex-span"><i>t</i></span> <span class="tex-font-style-underline">Т-prime</span>, if <span class="tex-span"><i>t</i></span> has exactly three distinct positive divisors.</p><p>You are given an array of <span class="tex-span"><i>n</i></span> positive integers. For each of them determine whether it is Т-prime or not.</p></div><div class="input-specification"><p>The first line contains a single positive integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), showing how many numbers are in the array. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is advised to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines: the <span class="tex-span"><i>i</i></span>-th line should contain "<span class="tex-font-style-tt">YES</span>" (without the quotes), if number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is Т-prime, and "<span class="tex-font-style-tt">NO</span>" (without the quotes), if it isn't.</p></div>

## Input

<p>The first line contains a single positive integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), showing how many numbers are in the array. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is advised to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines: the <span class="tex-span"><i>i</i></span>-th line should contain "<span class="tex-font-style-tt">YES</span>" (without the quotes), if number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is Т-prime, and "<span class="tex-font-style-tt">NO</span>" (without the quotes), if it isn't.</p>





```input1
3
4 5 6

```




```output1
YES
NO
NO

```



## Note

<p>The given test has three numbers. The first number 4 has exactly three divisors — 1, 2 and 4, thus the answer for this number is "<span class="tex-font-style-tt">YES</span>". The second number 5 has two divisors (1 and 5), and the third number 6 has four divisors (1, 2, 3, 6), hence the answer for them is "<span class="tex-font-style-tt">NO</span>".</p>
