## Description

<div><p>You've got another problem dealing with arrays. Let's consider an arbitrary sequence containing <span class="tex-span"><i>n</i></span> (not necessarily different) integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. We are interested in all possible pairs of numbers (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>), (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>). In other words, let's consider all <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> pairs of numbers, picked from the given array.</p><p>For example, in sequence <span class="tex-span"><i>a</i> = {3, 1, 5}</span> are <span class="tex-span">9</span> pairs of numbers: <span class="tex-span">(3, 3), (3, 1), (3, 5), (1, 3), (1, 1), (1, 5), (5, 3), (5, 1), (5, 5)</span>.</p><p>Let's sort all resulting pairs lexicographically by non-decreasing. Let us remind you that pair (<span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index">1</sub></span>) is <span class="tex-font-style-underline">lexicographically less</span> than pair (<span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>q</i><sub class="lower-index">2</sub></span>) only if either <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> &lt; <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, or <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> = <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index">1</sub></span> &lt; <span class="tex-span"><i>q</i><sub class="lower-index">2</sub></span>.</p><p>Then the sequence, mentioned above, will be sorted like that: <span class="tex-span">(1, 1), (1, 3), (1, 5), (3, 1), (3, 3), (3, 5), (5, 1), (5, 3), (5, 5)</span></p><p>Let's number all the pair in the sorted list from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span>. Your task is formulated like this: you should find the <span class="tex-span"><i>k</i></span>-th pair in the ordered list of all possible pairs of the array you've been given.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>n</i><sup class="upper-index">2</sup></span>). The second line contains the array containing <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The numbers in the array can coincide. All numbers are separated with spaces.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span>, streams or the <span class="tex-font-style-tt">%I64d</span> specificator instead.</p></div><div class="output-specification"><p>In the single line print two numbers — the sought <span class="tex-span"><i>k</i></span>-th pair.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>n</i><sup class="upper-index">2</sup></span>). The second line contains the array containing <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The numbers in the array can coincide. All numbers are separated with spaces.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span>, streams or the <span class="tex-font-style-tt">%I64d</span> specificator instead.</p>

## Output

<p>In the single line print two numbers — the sought <span class="tex-span"><i>k</i></span>-th pair.</p>





```input1
2 4
2 1

```




```input2
3 2
3 1 5

```




```output1
2 2

```




```output2
1 3

```



## Note

<p>In the first sample the sorted sequence for the given array looks as: <span class="tex-span">(1, 1), (1, 2), (2, 1), (2, 2)</span>. The <span class="tex-span">4</span>-th of them is pair <span class="tex-span">(2, 2)</span>.</p><p>The sorted sequence for the array from the second sample is given in the statement. The <span class="tex-span">2</span>-nd pair there is <span class="tex-span">(1, 3)</span>.</p>
