## Description

<div><p>Xenia the beginner programmer has a sequence <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> non-negative integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">2<sup class="upper-index"><i>n</i></sup></sub></span>. Xenia is currently studying bit operations. To better understand how they work, Xenia decided to calculate some value <span class="tex-span"><i>v</i></span> for <span class="tex-span"><i>a</i></span>.</p><p>Namely, it takes several iterations to calculate value <span class="tex-span"><i>v</i></span>. At the first iteration, Xenia writes a new sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>&nbsp;<i>or</i>&nbsp;<i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>&nbsp;<i>or</i>&nbsp;<i>a</i><sub class="lower-index">4</sub>, ..., <i>a</i><sub class="lower-index">2<sup class="upper-index"><i>n</i></sup> - 1</sub>&nbsp;<i>or</i>&nbsp;<i>a</i><sub class="lower-index">2<sup class="upper-index"><i>n</i></sup></sub></span>, consisting of <span class="tex-span">2<sup class="upper-index"><i>n</i> - 1</sup></span> elements. In other words, she writes down the bit-wise OR of adjacent elements of sequence <span class="tex-span"><i>a</i></span>. At the second iteration, Xenia writes the bitwise <span class="tex-font-style-bf">exclusive</span> OR of adjacent elements of the sequence obtained after the first iteration. At the third iteration Xenia writes the bitwise OR of the adjacent elements of the sequence obtained after the second iteration. And so on; the operations of bitwise exclusive OR and bitwise OR alternate. In the end, she obtains a sequence consisting of one element, and that element is <span class="tex-span"><i>v</i></span>.</p><p>Let's consider an example. Suppose that sequence <span class="tex-span"><i>a</i> = (1, 2, 3, 4)</span>. Then let's write down all the transformations <span class="tex-span">(1, 2, 3, 4)</span> <span class="tex-span"> → </span> <span class="tex-span">(1&nbsp;<i>or</i>&nbsp;2 = 3, 3&nbsp;<i>or</i>&nbsp;4 = 7)</span> <span class="tex-span"> → </span> <span class="tex-span">(3&nbsp;<i>xor</i>&nbsp;7 = 4)</span>. The result is <span class="tex-span"><i>v</i> = 4</span>.</p><p>You are given Xenia's initial sequence. But to calculate value <span class="tex-span"><i>v</i></span> for a given sequence would be too easy, so you are given additional <span class="tex-span"><i>m</i></span> queries. Each query is a pair of integers <span class="tex-span"><i>p</i>, <i>b</i></span>. Query <span class="tex-span"><i>p</i>, <i>b</i></span> means that you need to perform the assignment <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i></sub> = <i>b</i></span>. After each query, you need to print the new value <span class="tex-span"><i>v</i></span> for the new sequence <span class="tex-span"><i>a</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 17, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">2<sup class="upper-index"><i>n</i></sup></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup>)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains queries. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 2<sup class="upper-index"><i>n</i></sup>, 0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>i</i></span>-th integer denotes value <span class="tex-span"><i>v</i></span> for sequence <span class="tex-span"><i>a</i></span> after the <span class="tex-span"><i>i</i></span>-th query.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 17, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">2<sup class="upper-index"><i>n</i></sup></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup>)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains queries. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 2<sup class="upper-index"><i>n</i></sup>, 0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>i</i></span>-th integer denotes value <span class="tex-span"><i>v</i></span> for sequence <span class="tex-span"><i>a</i></span> after the <span class="tex-span"><i>i</i></span>-th query.</p>





```input1
2 4
1 6 3 5
1 4
3 4
1 2
1 2

```




```output1
1
3
3
3

```



## Note

<p>For more information on the bit operations, you can follow this link: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Bitwise_operation</span></p>
