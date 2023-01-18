## Description

<div><p>A number is called <span class="tex-font-style-it">quasibinary</span> if its decimal representation contains only digits 0 or 1. For example, numbers 0, 1, 101, 110011&nbsp;— are quasibinary and numbers 2, 12, 900 are not.</p><p>You are given a positive integer <span class="tex-span"><i>n</i></span>. Represent it as a sum of minimum number of quasibinary numbers.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the minimum number of numbers in the representation of number <span class="tex-span"><i>n</i></span> as a sum of quasibinary numbers.</p><p>In the second line print <span class="tex-span"><i>k</i></span> numbers — the elements of the sum. All these numbers should be quasibinary according to the definition above, their sum should equal <span class="tex-span"><i>n</i></span>. Do not have to print the leading zeroes in the numbers. The order of numbers doesn't matter. If there are multiple possible representations, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the minimum number of numbers in the representation of number <span class="tex-span"><i>n</i></span> as a sum of quasibinary numbers.</p><p>In the second line print <span class="tex-span"><i>k</i></span> numbers — the elements of the sum. All these numbers should be quasibinary according to the definition above, their sum should equal <span class="tex-span"><i>n</i></span>. Do not have to print the leading zeroes in the numbers. The order of numbers doesn't matter. If there are multiple possible representations, you are allowed to print any of them.</p>





```input1
9

```




```input2
32

```




```output1
9
1 1 1 1 1 1 1 1 1 

```




```output2
3
10 11 11 

```


