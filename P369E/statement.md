## Description

<div><p>Valera loves segments. He has recently come up with one interesting problem.</p><p>The <span class="tex-span"><i>Ox</i></span> axis of coordinates has <span class="tex-span"><i>n</i></span> segments, the <span class="tex-span"><i>i</i></span>-th segment starts in position <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and ends in position <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (we will mark it as <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>). Your task is to process <span class="tex-span"><i>m</i></span> queries, each consists of number <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>i</i></sub></span> and a set of <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>i</i></sub></span> coordinates of points located on the <span class="tex-span"><i>Ox</i></span> axis. The answer to the query is the number of segments, such that each of them contains at least one point from the query. Segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> <span class="tex-font-style-it">contains</span> point <span class="tex-span"><i>q</i></span>, if <span class="tex-span"><i>l</i> ≤ <i>q</i> ≤ <i>r</i></span>.</p><p>Valera found the solution of this problem too difficult. So he asked you to help him. Help Valera. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of segments on the axis of coordinates and the number of queries. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the segments. The <span class="tex-span"><i>i</i></span>-th line contains two positive integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the borders of the <span class="tex-span"><i>i</i></span>-th segment.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the description of the queries, one per line. Each line starts from integer <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>cnt</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of points in the <span class="tex-span"><i>i</i></span>-th query. Then the line contains <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>i</i></sub></span> distinct positive integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>cnt</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>cnt</i><sub class="lower-index"><i>i</i></sub></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of points in the <span class="tex-span"><i>i</i></span>-th query.</p><p>It is guaranteed that the total number of points in all queries doesn't exceed <span class="tex-span">3·10<sup class="upper-index">5</sup></span>. </p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> non-negative integers, where the <span class="tex-span"><i>i</i></span>-th number is the response to the <span class="tex-span"><i>i</i></span>-th query.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of segments on the axis of coordinates and the number of queries. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the segments. The <span class="tex-span"><i>i</i></span>-th line contains two positive integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the borders of the <span class="tex-span"><i>i</i></span>-th segment.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the description of the queries, one per line. Each line starts from integer <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>cnt</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of points in the <span class="tex-span"><i>i</i></span>-th query. Then the line contains <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>i</i></sub></span> distinct positive integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>cnt</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>cnt</i><sub class="lower-index"><i>i</i></sub></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the coordinates of points in the <span class="tex-span"><i>i</i></span>-th query.</p><p>It is guaranteed that the total number of points in all queries doesn't exceed <span class="tex-span">3·10<sup class="upper-index">5</sup></span>. </p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> non-negative integers, where the <span class="tex-span"><i>i</i></span>-th number is the response to the <span class="tex-span"><i>i</i></span>-th query.</p>





```input1
3 3
1 3
4 5
6 7
3 1 4 7
2 4 5
1 8

```




```output1
3
1
0

```


