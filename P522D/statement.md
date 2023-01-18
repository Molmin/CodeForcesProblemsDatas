## Description

<div><p>You are given sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>m</i></span> queries <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>). For each query you need to print the minimum distance between such pair of elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span"><i>x</i> ≠ <i>y</i></span>), that:</p><ul> <li> both indexes of the elements lie within range [<span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span>], that is, <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>x</i>, <i>y</i> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub></span>; </li><li> the values of the elements are equal, that is <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub> = <i>a</i><sub class="lower-index"><i>y</i></sub></span>. </li></ul><p>The text above understands distance as <span class="tex-span">|<i>x</i> - <i>y</i>|</span>.</p></div><div class="input-specification"><p>The first line of the input contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the length of the sequence and the number of queries, correspondingly. </p><p>The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the queries, one per line. Each query is given by a pair of numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the indexes of the query range limits.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the answers to each query. If there is no valid match for some query, please print <span class="tex-font-style-tt">-1</span> as an answer to this query.</p></div>

## Input

<p>The first line of the input contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the length of the sequence and the number of queries, correspondingly. </p><p>The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the queries, one per line. Each query is given by a pair of numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the indexes of the query range limits.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the answers to each query. If there is no valid match for some query, please print <span class="tex-font-style-tt">-1</span> as an answer to this query.</p>





```input1
5 3
1 1 2 3 2
1 5
2 4
3 5

```




```input2
6 5
1 2 1 3 2 3
4 6
1 3
2 5
2 4
1 6

```




```output1
1
-1
2

```




```output2
2
2
3
-1
2

```


