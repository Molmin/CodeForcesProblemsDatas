## Description

<div><p>Recently, the bear started studying data structures and faced the following problem.</p><p>You are given a sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> queries, each of them is characterized by two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span>. Let's introduce <span class="tex-span"><i>f</i>(<i>p</i>)</span> to represent the number of such indexes <span class="tex-span"><i>k</i></span>, that <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span> is divisible by <span class="tex-span"><i>p</i></span>. The answer to the query <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> is the sum: <img align="middle" class="tex-formula" src="file://QqUBk1fA.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>S</i>(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> is a set of prime numbers from segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> (both borders are included in the segment).</p><p>Help the bear cope with the problem.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(2 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup>)</span>. The numbers are not necessarily distinct.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 50000)</span>. Each of the following <span class="tex-span"><i>m</i></span> lines contains a pair of space-separated integers, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(2 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup>)</span> — the numbers that characterize the current query.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the answers to the queries on the order the queries appear in the input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(2 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup>)</span>. The numbers are not necessarily distinct.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 50000)</span>. Each of the following <span class="tex-span"><i>m</i></span> lines contains a pair of space-separated integers, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(2 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup>)</span> — the numbers that characterize the current query.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the answers to the queries on the order the queries appear in the input.</p>





```input1
6
5 5 7 10 14 15
3
2 11
3 12
4 4

```




```input2
7
2 3 5 7 11 4 8
2
8 10
2 123

```




```output1
9
7
0

```




```output2
0
7

```



## Note

<p>Consider the first sample. Overall, the first sample has 3 queries.</p><ol> <li> The first query <span class="tex-span"><i>l</i> = 2</span>, <span class="tex-span"><i>r</i> = 11</span> comes. You need to count <span class="tex-span"><i>f</i>(2) + <i>f</i>(3) + <i>f</i>(5) + <i>f</i>(7) + <i>f</i>(11) = 2 + 1 + 4 + 2 + 0 = 9</span>. </li><li> The second query comes <span class="tex-span"><i>l</i> = 3</span>, <span class="tex-span"><i>r</i> = 12</span>. You need to count <span class="tex-span"><i>f</i>(3) + <i>f</i>(5) + <i>f</i>(7) + <i>f</i>(11) = 1 + 4 + 2 + 0 = 7</span>. </li><li> The third query comes <span class="tex-span"><i>l</i> = 4</span>, <span class="tex-span"><i>r</i> = 4</span>. As this interval has no prime numbers, then the sum equals 0. </li></ol>
