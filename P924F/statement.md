## Description

<div><p>We call a positive integer <span class="tex-span"><i>x</i></span> a <span class="tex-span"><i>k</i></span>-beautiful integer if and only if it is possible to split the multiset of its digits in the decimal representation into two subsets such that the difference between the sum of digits in one subset and the sum of digits in the other subset is <span class="tex-font-style-bf">less than or equal to</span> <span class="tex-span"><i>k</i></span>. Each digit should belong to exactly one subset after the split.</p><p>There are <span class="tex-span"><i>n</i></span> queries for you. Each query is described with three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span>, which mean that you are asked how many integers <span class="tex-span"><i>x</i></span> between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (inclusive) are <span class="tex-span"><i>k</i></span>-beautiful.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>), indicating the number of queries.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines describes a query, containing three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 9</span>).</p></div><div class="output-specification"><p>For each query print a single number&nbsp;— the answer to the query.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>), indicating the number of queries.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines describes a query, containing three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 9</span>).</p>

## Output

<p>For each query print a single number&nbsp;— the answer to the query.</p>





```input1
10
1 100 0
1 100 1
1 100 2
1 100 3
1 100 4
1 100 5
1 100 6
1 100 7
1 100 8
1 100 9

```




```input2
10
1 1000 0
1 1000 1
1 1000 2
1 1000 3
1 1000 4
1 1000 5
1 1000 6
1 1000 7
1 1000 8
1 1000 9

```




```output1
9
28
44
58
70
80
88
94
98
100

```




```output2
135
380
573
721
830
906
955
983
996
1000

```



## Note

<p>If <span class="tex-span">1 ≤ <i>x</i> ≤ 9</span>, integer <span class="tex-span"><i>x</i></span> is <span class="tex-span"><i>k</i></span>-beautiful if and only if <span class="tex-span"><i>x</i> ≤ <i>k</i></span>.</p><p>If <span class="tex-span">10 ≤ <i>x</i> ≤ 99</span>, integer <span class="tex-span"><i>x</i> = 10<i>a</i> + <i>b</i></span> is <span class="tex-span"><i>k</i></span>-beautiful if and only if <span class="tex-span">|<i>a</i> - <i>b</i>| ≤ <i>k</i></span>, where <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are integers between <span class="tex-span">0</span> and <span class="tex-span">9</span>, inclusive.</p><p><span class="tex-span">100</span> is <span class="tex-span"><i>k</i></span>-beautiful if and only if <span class="tex-span"><i>k</i> ≥ 1</span>.</p>
