## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Denote this list of integers as <span class="tex-span"><i>T</i></span>.</p><p>Let <span class="tex-span"><i>f</i>(<i>L</i>)</span> be a function that takes in a non-empty list of integers <span class="tex-span"><i>L</i></span>.</p><p>The function will output another integer as follows: </p><ul> <li> First, all integers in <span class="tex-span"><i>L</i></span> are padded with leading zeros so they are all the same length as the maximum length number in <span class="tex-span"><i>L</i></span>. </li><li> We will construct a string where the <span class="tex-span"><i>i</i></span>-th character is the minimum of the <span class="tex-span"><i>i</i></span>-th character in padded input numbers. </li><li> The output is the number representing the string interpreted in base 10. </li></ul><p>For example <span class="tex-span"><i>f</i>(10, 9) = 0</span>, <span class="tex-span"><i>f</i>(123, 321) = 121</span>, <span class="tex-span"><i>f</i>(530, 932, 81) = 30</span>.</p><p>Define the function </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://1tH7mfQ2.png" style="max-width: 100.0%;max-height: 100.0%;"></center> Here, <img align="middle" class="tex-formula" src="file://CLE0YXRw.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes a subsequence.<p>In other words, <span class="tex-span"><i>G</i>(<i>x</i>)</span> is the sum of squares of sum of elements of nonempty subsequences of <span class="tex-span"><i>T</i></span> that evaluate to <span class="tex-span"><i>x</i></span> when plugged into <span class="tex-span"><i>f</i></span> modulo <span class="tex-span">1 000 000 007</span>, then multiplied by <span class="tex-span"><i>x</i></span>. The last multiplication is not modded. </p><p>You would like to compute <span class="tex-span"><i>G</i>(0), <i>G</i>(1), ..., <i>G</i>(999 999)</span>. To reduce the output size, print the value <img align="middle" class="tex-formula" src="file://Ceenxt49.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://CgDCZxKh.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the bitwise XOR operator.</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the size of list <span class="tex-span"><i>T</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 999 999</span>)&nbsp;— the elements of the list. </p></div><div class="output-specification"><p>Output a single integer, the answer to the problem.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the size of list <span class="tex-span"><i>T</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 999 999</span>)&nbsp;— the elements of the list. </p>

## Output

<p>Output a single integer, the answer to the problem.</p>





```input1
3
123 321 555

```




```input2
1
999999

```




```input3
10
1 1 1 1 1 1 1 1 1 1

```




```output1
292711924

```




```output2
997992010006992

```




```output3
28160

```



## Note

<p>For the first sample, the nonzero values of <span class="tex-span"><i>G</i></span> are <span class="tex-span"><i>G</i>(121) = 144 611 577</span>, <span class="tex-span"><i>G</i>(123) = 58 401 999</span>, <span class="tex-span"><i>G</i>(321) = 279 403 857</span>, <span class="tex-span"><i>G</i>(555) = 170 953 875</span>. The bitwise XOR of these numbers is equal to <span class="tex-span">292 711 924</span>.</p><p>For example, <img align="middle" class="tex-formula" src="file://VsS58vc2.png" style="max-width: 100.0%;max-height: 100.0%;">, since the subsequences <span class="tex-span">[123]</span> and <span class="tex-span">[123, 555]</span> evaluate to <span class="tex-span">123</span> when plugged into <span class="tex-span"><i>f</i></span>.</p><p>For the second sample, we have <img align="middle" class="tex-formula" src="file://0IHA1ZrK.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>For the last sample, we have <img align="middle" class="tex-formula" src="file://xL9FC3bN.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://CXVn8khv.png" style="max-width: 100.0%;max-height: 100.0%;"> is the binomial coefficient.</p>
