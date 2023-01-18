## Description

<div><p>We are given a permutation sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Let's assume that in one second, we can choose some disjoint pairs <span class="tex-span">(<i>u</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">1</sub>), (<i>u</i><sub class="lower-index">2</sub>, <i>v</i><sub class="lower-index">2</sub>), ..., (<i>u</i><sub class="lower-index"><i>k</i></sub>, <i>v</i><sub class="lower-index"><i>k</i></sub>)</span> and swap all <span class="tex-span"><i>a</i><sub class="lower-index"><i>u</i><sub class="lower-index"><i>i</i></sub></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i><sub class="lower-index"><i>i</i></sub></sub></span> for every <span class="tex-span"><i>i</i></span> at the same time (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> &lt; <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). The pairs are disjoint if every <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> are different from each other.</p><p>We want to sort the sequence completely in increasing order as fast as possible. Given the initial permutation, calculate the number of ways to achieve this. Two ways are different if and only if there is a time <span class="tex-span"><i>t</i></span>, such that the set of pairs used for swapping at that time are different as sets (so ordering of pairs doesn't matter). If the given permutation is already sorted, it takes no time to sort, so the number of ways to sort it is <span class="tex-span">1</span>.</p><p>To make the problem more interesting, we have <span class="tex-span"><i>k</i></span> holes inside the permutation. So exactly <span class="tex-span"><i>k</i></span> numbers of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> are not yet determined. For every possibility of filling the holes, calculate the number of ways, and print the total sum of these values modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 12)</span>. The second line contains the permutation sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. If a number is not yet determined, it is denoted as <span class="tex-span">0</span>. There are exactly <span class="tex-span"><i>k</i></span> zeroes. All the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> that aren't equal to zero are distinct.</p></div><div class="output-specification"><p>Print the total sum of the number of ways modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 12)</span>. The second line contains the permutation sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. If a number is not yet determined, it is denoted as <span class="tex-span">0</span>. There are exactly <span class="tex-span"><i>k</i></span> zeroes. All the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> that aren't equal to zero are distinct.</p>

## Output

<p>Print the total sum of the number of ways modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
5 0
1 5 2 4 3

```




```input2
5 2
1 0 2 4 0

```




```output1
6

```




```output2
7

```


