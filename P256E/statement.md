## Description

<div><p>Little Maxim loves interesting problems. He decided to share one such problem with you. </p><p>Initially there is an array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> zeroes. The elements of the array are indexed, starting from 1. Then follow queries to change array <span class="tex-span"><i>a</i></span>. Each query is characterized by two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span>. In the answer to the query we should make the <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>-th array element equal <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>a</i><sub class="lower-index"><i>v</i><sub class="lower-index"><i>i</i></sub></sub> = <i>t</i><sub class="lower-index"><i>i</i></sub>;&nbsp;1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p><p>Maxim thinks that some pairs of integers <span class="tex-span">(<i>x</i>, <i>y</i>)</span> are good and some are not. Maxim thinks that array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers, is lucky, if for all integer <span class="tex-span"><i>i</i></span>, <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i> - 1)</span> the pair of integers <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>)</span> — is good. Note that the order of numbers in the pairs is important, that is, specifically, <span class="tex-span">(1, 2) ≠ (2, 1)</span>.</p><p>After each query to change array <span class="tex-span"><i>a</i></span> Maxim wants to know, how many ways there are to replace all zeroes in array <span class="tex-span"><i>a</i></span> with integers from one to three so as to make the resulting array (without zeroes) lucky. Of course, distinct zeroes can be replaced by distinct integers.</p><p>Maxim told you the sequence of queries and all pairs of integers he considers lucky. Help Maxim, solve this problem for him.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 77777)</span> — the number of elements in the array and the number of commands.</p><p>The next three lines contain matrix <span class="tex-span"><i>w</i></span>, consisting only of zeroes and ones; the <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th of these lines — <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. If <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ 3)</span>, then pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is good, otherwise it is not good. Matrix does not have to be symmetric relative to the main diagonal.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3)</span> — the queries to change the array.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>i</i></span>-th number should equal to the number of ways to replace all zeroes in array <span class="tex-span"><i>a</i></span> (changed after the <span class="tex-span"><i>i</i></span>-th query) by integers from one to three so as to make the resulting array (without zeroes) lucky. Separate the numbers by whitespaces. As the answers can be rather large, print the remainder from dividing them by <span class="tex-span">777777777</span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 77777)</span> — the number of elements in the array and the number of commands.</p><p>The next three lines contain matrix <span class="tex-span"><i>w</i></span>, consisting only of zeroes and ones; the <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th of these lines — <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. If <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ 3)</span>, then pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is good, otherwise it is not good. Matrix does not have to be symmetric relative to the main diagonal.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3)</span> — the queries to change the array.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>i</i></span>-th number should equal to the number of ways to replace all zeroes in array <span class="tex-span"><i>a</i></span> (changed after the <span class="tex-span"><i>i</i></span>-th query) by integers from one to three so as to make the resulting array (without zeroes) lucky. Separate the numbers by whitespaces. As the answers can be rather large, print the remainder from dividing them by <span class="tex-span">777777777</span>.</p>





```input1
3 10
1 1 0
1 0 0
1 1 1
1 1
1 3
2 2
3 0
2 1
3 0
3 1
2 0
3 1
1 0

```




```output1
3
6
1
1
2
2
1
3
3
6

```


