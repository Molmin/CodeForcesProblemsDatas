## Description

<div><p>A <span class="tex-span"><i>k</i></span>-multiple free set is a set of integers where there is no pair of integers where one is equal to another integer multiplied by <span class="tex-span"><i>k</i></span>. That is, there are no two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(<i>x</i> &lt; <i>y</i>)</span> from the set, such that <span class="tex-span"><i>y</i> = <i>x</i>·<i>k</i></span>.</p><p>You're given a set of <span class="tex-span"><i>n</i></span> distinct positive integers. Your task is to find the size of it's largest <span class="tex-span"><i>k</i></span>-multiple free subset.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains a list of <span class="tex-span"><i>n</i></span> distinct positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>All the numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>On the only line of the output print the size of the largest <span class="tex-span"><i>k</i></span>-multiple free subset of <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains a list of <span class="tex-span"><i>n</i></span> distinct positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>All the numbers in the lines are separated by single spaces.</p>

## Output

<p>On the only line of the output print the size of the largest <span class="tex-span"><i>k</i></span>-multiple free subset of <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span>.</p>





```input1
6 2
2 3 6 5 4 10

```




```output1
3

```



## Note

<p>In the sample input one of the possible maximum 2-multiple free subsets is {4, 5, 6}.</p>
