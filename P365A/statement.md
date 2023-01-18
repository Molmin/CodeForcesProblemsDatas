## Description

<div><p>Let's call a number <span class="tex-span"><i>k</i></span>-good if it contains all digits not exceeding <span class="tex-span"><i>k</i></span> (<span class="tex-span">0, ..., <i>k</i></span>). You've got a number <span class="tex-span"><i>k</i></span> and an array <span class="tex-span"><i>a</i></span> containing <span class="tex-span"><i>n</i></span> numbers. Find out how many <span class="tex-span"><i>k</i></span>-good numbers are in <span class="tex-span"><i>a</i></span> (count each number every time it occurs in array <span class="tex-span"><i>a</i></span>).</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 9</span>). The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> without leading zeroes (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print a single integer — the number of <span class="tex-span"><i>k</i></span>-good numbers in <span class="tex-span"><i>a</i></span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 9</span>). The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> without leading zeroes (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print a single integer — the number of <span class="tex-span"><i>k</i></span>-good numbers in <span class="tex-span"><i>a</i></span>.</p>





```input1
10 6
1234560
1234560
1234560
1234560
1234560
1234560
1234560
1234560
1234560
1234560

```




```input2
2 1
1
10

```




```output1
10

```




```output2
1

```


