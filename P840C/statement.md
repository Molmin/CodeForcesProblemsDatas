## Description

<div><p>A year ago on the bench in public park Leha found an array of <span class="tex-span"><i>n</i></span> numbers. Leha believes that permutation <span class="tex-span"><i>p</i></span> is right if for all <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span> condition, that <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub>·<i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></sub></span> is not perfect square, holds. Leha wants to find number of right permutations modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>First line of input data contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — length of the array.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — found array.</p></div><div class="output-specification"><p>Output single integer — number of right permutations modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>First line of input data contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — length of the array.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — found array.</p>

## Output

<p>Output single integer — number of right permutations modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
1 2 4

```




```input2
7
5 2 4 2 4 1 1

```




```output1
2

```




```output2
144

```



## Note

<p>For first example:</p><p><span class="tex-span">[1, 2, 4]</span> — right permutation, because <span class="tex-span">2</span> and <span class="tex-span">8</span> are not perfect squares.</p><p><span class="tex-span">[1, 4, 2]</span> — wrong permutation, because <span class="tex-span">4</span> is square of <span class="tex-span">2</span>.</p><p><span class="tex-span">[2, 1, 4]</span> — wrong permutation, because <span class="tex-span">4</span> is square of <span class="tex-span">2</span>.</p><p><span class="tex-span">[2, 4, 1]</span> — wrong permutation, because <span class="tex-span">4</span> is square of <span class="tex-span">2</span>.</p><p><span class="tex-span">[4, 1, 2]</span> — wrong permutation, because <span class="tex-span">4</span> is square of <span class="tex-span">2</span>.</p><p><span class="tex-span">[4, 2, 1]</span> — right permutation, because <span class="tex-span">8</span> and <span class="tex-span">2</span> are not perfect squares.</p>
