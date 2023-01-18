## Description

<div><p>An array of positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> is given. Let us consider its arbitrary subarray <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>..., <i>a</i><sub class="lower-index"><i>r</i></sub></span>, where <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>. For every positive integer <span class="tex-span"><i>s</i></span> denote by <span class="tex-span"><i>K</i><sub class="lower-index"><i>s</i></sub></span> the number of occurrences of <span class="tex-span"><i>s</i></span> into the subarray. We call the <span class="tex-font-style-it">power</span> of the subarray the sum of products <span class="tex-span"><i>K</i><sub class="lower-index"><i>s</i></sub>·<i>K</i><sub class="lower-index"><i>s</i></sub>·<i>s</i></span> for every positive integer <span class="tex-span"><i>s</i></span>. The sum contains only finite number of nonzero summands as the number of different values in the array is indeed finite.</p><p>You should calculate the power of <span class="tex-span"><i>t</i></span> given subarrays.</p></div><div class="input-specification"><p>First line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i> ≤ 200000</span>) — the array length and the number of queries correspondingly.</p><p>Second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array.</p><p>Next <span class="tex-span"><i>t</i></span> lines contain two positive integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) each — the indices of the left and the right ends of the corresponding subarray.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>t</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line of the output should contain single positive integer — the power of the <span class="tex-span"><i>i</i></span>-th query subarray.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> stream (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>First line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i> ≤ 200000</span>) — the array length and the number of queries correspondingly.</p><p>Second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the elements of the array.</p><p>Next <span class="tex-span"><i>t</i></span> lines contain two positive integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) each — the indices of the left and the right ends of the corresponding subarray.</p>

## Output

<p>Output <span class="tex-span"><i>t</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line of the output should contain single positive integer — the power of the <span class="tex-span"><i>i</i></span>-th query subarray.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> stream (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
3 2
1 2 1
1 2
1 3

```




```input2
8 3
1 1 2 2 1 3 1 1
2 7
1 6
2 7

```




```output1
3
6

```




```output2
20
20
20

```



## Note

<p>Consider the following array (see the second sample) and its [2, 7] subarray (elements of the subarray are colored): </p><center><img class="tex-graphics" src="file://uIxVtkWn.png" style="max-width: 100.0%;max-height: 100.0%;"></center> Then <span class="tex-span"><i>K</i><sub class="lower-index">1</sub> = 3</span>, <span class="tex-span"><i>K</i><sub class="lower-index">2</sub> = 2</span>, <span class="tex-span"><i>K</i><sub class="lower-index">3</sub> = 1</span>, so the power is equal to <span class="tex-span">3<sup class="upper-index">2</sup>·1 + 2<sup class="upper-index">2</sup>·2 + 1<sup class="upper-index">2</sup>·3 = 20</span>.
