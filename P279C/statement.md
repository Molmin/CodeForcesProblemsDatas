## Description

<div><p>You've got an array, consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Also, you've got <span class="tex-span"><i>m</i></span> queries, the <span class="tex-span"><i>i</i></span>-th query is described by two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span>. Numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> define a subsegment of the original array, that is, the sequence of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub>, <i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub> + 1</sub>, <i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub> + 2</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub></span>. For each query you should check whether the corresponding segment is a ladder. </p><p>A <span class="tex-font-style-it">ladder</span> is a sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span>, such that it first doesn't decrease, then doesn't increase. In other words, there is such integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>k</i>)</span>, that the following inequation fulfills: <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> ≤ <i>b</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>b</i><sub class="lower-index"><i>x</i></sub> ≥ <i>b</i><sub class="lower-index"><i>x</i> + 1</sub> ≥ <i>b</i><sub class="lower-index"><i>x</i> + 2</sub>... ≥ <i>b</i><sub class="lower-index"><i>k</i></sub></span>. Note that the non-decreasing and the non-increasing sequences are also considered ladders.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of array elements and the number of queries. The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> stands for the <span class="tex-span"><i>i</i></span>-th array element.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the description of the queries. The <span class="tex-span"><i>i</i></span>-th line contains the description of the <span class="tex-span"><i>i</i></span>-th query, consisting of two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the boundaries of the subsegment of the initial array.</p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, in the <span class="tex-span"><i>i</i></span>-th line print word "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if the subsegment that corresponds to the <span class="tex-span"><i>i</i></span>-th query is the ladder, or word "<span class="tex-font-style-tt">No</span>" (without the quotes) otherwise. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of array elements and the number of queries. The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> stands for the <span class="tex-span"><i>i</i></span>-th array element.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the description of the queries. The <span class="tex-span"><i>i</i></span>-th line contains the description of the <span class="tex-span"><i>i</i></span>-th query, consisting of two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the boundaries of the subsegment of the initial array.</p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, in the <span class="tex-span"><i>i</i></span>-th line print word "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if the subsegment that corresponds to the <span class="tex-span"><i>i</i></span>-th query is the ladder, or word "<span class="tex-font-style-tt">No</span>" (without the quotes) otherwise. </p>





```input1
8 6
1 2 1 3 3 5 2 1
1 3
2 3
2 4
8 8
1 4
5 8

```




```output1
Yes
Yes
No
Yes
No
Yes

```


