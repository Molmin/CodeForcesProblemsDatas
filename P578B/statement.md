## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. You can perform at most <span class="tex-span"><i>k</i></span> operations. For each operation you can multiply one of the numbers by <span class="tex-span"><i>x</i></span>. We want to make <img align="middle" class="tex-formula" src="file://UKjL8uBQ.png" style="max-width: 100.0%;max-height: 100.0%;"> as large as possible, where <img align="middle" class="tex-formula" src="file://iL9vkoQL.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the bitwise OR. </p><p>Find the maximum possible value of <img align="middle" class="tex-formula" src="file://r44IrvXe.png" style="max-width: 100.0%;max-height: 100.0%;"> after performing at most <span class="tex-span"><i>k</i></span> operations optimally.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10</span>, <span class="tex-span">2 ≤ <i>x</i> ≤ 8</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output the maximum value of a bitwise OR of sequence elements after performing operations.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10</span>, <span class="tex-span">2 ≤ <i>x</i> ≤ 8</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output the maximum value of a bitwise OR of sequence elements after performing operations.</p>





```input1
3 1 2
1 1 1

```




```input2
4 2 3
1 2 4 8

```




```output1
3

```




```output2
79

```



## Note

<p>For the first sample, any possible choice of doing one operation will result the same three numbers <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span> so the result is <img align="middle" class="tex-formula" src="file://Riv9rg6J.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>For the second sample if we multiply <span class="tex-span">8</span> by <span class="tex-span">3</span> two times we'll get <span class="tex-span">72</span>. In this case the numbers will become <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">4</span>, <span class="tex-span">72</span> so the OR value will be <span class="tex-span">79</span> and is the largest possible result.</p>
