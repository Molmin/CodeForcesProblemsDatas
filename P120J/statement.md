## Description

<div><p>You are given a set of <span class="tex-span"><i>n</i></span> vectors on a plane. For each vector you are allowed to multiply any of its coordinates by <span class="tex-font-style-tt">-1</span>. Thus, each vector <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> = (<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> can be transformed into one of the following four vectors:</p><ul> <li> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">1</sup> = (<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, </li><li> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> = ( - <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, </li><li> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">3</sup> = (<i>x</i><sub class="lower-index"><i>i</i></sub>,  - <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, </li><li> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">4</sup> = ( - <i>x</i><sub class="lower-index"><i>i</i></sub>,  - <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. </li></ul> <p>You should find two vectors from the set and determine which of their coordinates should be multiplied by <span class="tex-font-style-tt">-1</span> so that the absolute value of the sum of the resulting vectors was minimally possible. More formally, you should choose two vectors <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i></span>) and two numbers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub> ≤ 4</span>), so that the value of the expression <span class="tex-span">|<i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>k</i><sub class="lower-index">1</sub></sup> + <i>v</i><sub class="lower-index"><i>j</i></sub><sup class="upper-index"><i>k</i><sub class="lower-index">2</sub></sup>|</span> were minimum.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Then <span class="tex-span"><i>n</i></span> lines contain vectors as pairs of integers "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span"> - 10000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>), one pair per line.</p></div><div class="output-specification"><p>Print on the first line four space-separated numbers "<span class="tex-span"><i>i</i></span> <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>j</i></span> <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span>" — the answer to the problem. If there are several variants the absolute value of whose sums is minimum, you can print any of them. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Then <span class="tex-span"><i>n</i></span> lines contain vectors as pairs of integers "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span"> - 10000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>), one pair per line.</p>

## Output

<p>Print on the first line four space-separated numbers "<span class="tex-span"><i>i</i></span> <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>j</i></span> <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span>" — the answer to the problem. If there are several variants the absolute value of whose sums is minimum, you can print any of them. </p>





```input1
5
-7 -3
9 0
-8 6
7 -8
4 -5

```




```input2
5
3 2
-4 7
-6 0
-8 4
5 1

```




```output1
3 2 4 2

```




```output2
3 4 5 4

```



## Note

<p>A sum of two vectors <span class="tex-span"><i>v</i> = (<i>x</i><sub class="lower-index"><i>v</i></sub>, <i>y</i><sub class="lower-index"><i>v</i></sub>)</span> and <span class="tex-span"><i>u</i> = (<i>x</i><sub class="lower-index"><i>u</i></sub>, <i>y</i><sub class="lower-index"><i>u</i></sub>)</span> is vector <span class="tex-span"><i>s</i> = <i>v</i> + <i>u</i> = (<i>x</i><sub class="lower-index"><i>v</i></sub> + <i>x</i><sub class="lower-index"><i>u</i></sub>, <i>y</i><sub class="lower-index"><i>v</i></sub> + <i>y</i><sub class="lower-index"><i>u</i></sub>)</span>.</p><p>An absolute value of vector <span class="tex-span"><i>v</i> = (<i>x</i>, <i>y</i>)</span> is number <img align="middle" class="tex-formula" src="file://y7XjivkQ.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>In the second sample there are several valid answers, such as:</p><p>(3 1 4 2), (3 1 4 4), (3 4 4 1), (3 4 4 3), (4 1 3 2), (4 1 3 4), (4 2 3 1).</p>
