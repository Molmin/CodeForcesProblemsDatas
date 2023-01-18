## Description

<div><p>The Little Elephant has array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> positive integers, indexed from 1 to <span class="tex-span"><i>n</i></span>. Let's denote the number with index <span class="tex-span"><i>i</i></span> as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The Little Elephant wants to count, how many pairs of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> are there, such that <span class="tex-span">1 ≤ <i>l</i> &lt; <i>r</i> ≤ <i>n</i></span> and sequence <span class="tex-span"><i>b</i> = <i>a</i><sub class="lower-index">1</sub><i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>l</i></sub><i>a</i><sub class="lower-index"><i>r</i></sub><i>a</i><sub class="lower-index"><i>r</i> + 1</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> has no more than <span class="tex-span"><i>k</i></span> inversions. </p><p>An <span class="tex-font-style-underline">inversion</span> in sequence <span class="tex-span"><i>b</i></span> is a pair of elements of the sequence <span class="tex-span"><i>b</i></span>, that change their relative order after a stable sorting of the sequence. In other words, an inversion is a pair of integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, such that <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ |<i>b</i>|</span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &gt; <i>b</i><sub class="lower-index"><i>j</i></sub></span>, where <span class="tex-span">|<i>b</i>|</span> is the length of sequence <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> is its <span class="tex-span"><i>j</i></span>-th element.</p><p>Help the Little Elephant and count the number of the described pairs.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the size of array <span class="tex-span"><i>a</i></span> and the maximum allowed number of inversions respectively. The next line contains <span class="tex-span"><i>n</i></span> positive integers, separated by single spaces, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — elements of array <span class="tex-span"><i>a</i></span>.</p><p>Please, do not use the %lld specifier to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specifier.</p></div><div class="output-specification"><p>In a single line print a single number — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the size of array <span class="tex-span"><i>a</i></span> and the maximum allowed number of inversions respectively. The next line contains <span class="tex-span"><i>n</i></span> positive integers, separated by single spaces, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — elements of array <span class="tex-span"><i>a</i></span>.</p><p>Please, do not use the %lld specifier to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specifier.</p>

## Output

<p>In a single line print a single number — the answer to the problem.</p>





```input1
3 1
1 3 2

```




```input2
5 2
1 3 2 1 7

```




```output1
3

```




```output2
6

```


