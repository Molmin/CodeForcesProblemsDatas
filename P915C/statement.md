## Description

<div><p>You are given two positive integer numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Permute (change order) of the digits of <span class="tex-span"><i>a</i></span> to construct maximal number not exceeding <span class="tex-span"><i>b</i></span>. No number in input and/or output can start with the digit <span class="tex-font-style-tt">0</span>.</p><p>It is allowed to leave <span class="tex-span"><i>a</i></span> as it is.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10<sup class="upper-index">18</sup></span>). The second line contains integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>). Numbers don't have leading zeroes. It is guaranteed that answer exists.</p></div><div class="output-specification"><p>Print the maximum possible number that is a permutation of digits of <span class="tex-span"><i>a</i></span> and is not greater than <span class="tex-span"><i>b</i></span>. The answer can't have any leading zeroes. It is guaranteed that the answer exists.</p><p>The number in the output should have exactly the same length as number <span class="tex-span"><i>a</i></span>. It should be a permutation of digits of <span class="tex-span"><i>a</i></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10<sup class="upper-index">18</sup></span>). The second line contains integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>). Numbers don't have leading zeroes. It is guaranteed that answer exists.</p>

## Output

<p>Print the maximum possible number that is a permutation of digits of <span class="tex-span"><i>a</i></span> and is not greater than <span class="tex-span"><i>b</i></span>. The answer can't have any leading zeroes. It is guaranteed that the answer exists.</p><p>The number in the output should have exactly the same length as number <span class="tex-span"><i>a</i></span>. It should be a permutation of digits of <span class="tex-span"><i>a</i></span>.</p>





```input1
123
222

```




```input2
3921
10000

```




```input3
4940
5000

```




```output1
213

```




```output2
9321

```




```output3
4940

```


