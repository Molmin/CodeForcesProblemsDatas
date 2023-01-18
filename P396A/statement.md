## Description

<div><p>You are given an integer <span class="tex-span"><i>m</i></span> as a product of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> <img align="middle" class="tex-formula" src="file://YjrcdnIB.png" style="max-width: 100.0%;max-height: 100.0%;">. Your task is to find the number of distinct decompositions of number <span class="tex-span"><i>m</i></span> into the product of <span class="tex-span"><i>n</i></span> ordered positive integers.</p><p>Decomposition into <span class="tex-span"><i>n</i></span> products, given in the input, must also be considered in the answer. As the answer can be very large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>). The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In a single line print a single number <span class="tex-span"><i>k</i></span> — the number of distinct decompositions of number <span class="tex-span"><i>m</i></span> into <span class="tex-span"><i>n</i></span> ordered multipliers modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>). The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In a single line print a single number <span class="tex-span"><i>k</i></span> — the number of distinct decompositions of number <span class="tex-span"><i>m</i></span> into <span class="tex-span"><i>n</i></span> ordered multipliers modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1
15

```




```input2
3
1 1 2

```




```input3
2
5 7

```




```output1
1

```




```output2
3

```




```output3
4

```



## Note

<p>In the second sample, the get a decomposition of number 2, you need any one number out of three to equal 2, and the rest to equal 1.</p><p>In the third sample, the possible ways of decomposing into ordered multipliers are [7,5], [5,7], [1,35], [35,1].</p><p>A decomposition of positive integer <span class="tex-span"><i>m</i></span> into <span class="tex-span"><i>n</i></span> ordered multipliers is a cortege of positive integers <span class="tex-span"><i>b</i> = {<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ... <i>b</i><sub class="lower-index"><i>n</i></sub>}</span> such that <img align="middle" class="tex-formula" src="file://Y0MUiB4w.png" style="max-width: 100.0%;max-height: 100.0%;">. Two decompositions <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> are considered different, if there exists index <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p>
