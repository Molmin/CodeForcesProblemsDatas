## Description

<div><p>Consider integer sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. You should run queries of two types:</p><ul> <li> The query format is "<span class="tex-span">0</span> <span class="tex-span"><i>i</i></span> <span class="tex-span"><i>val</i></span>". In reply to this query you should make the following assignment: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>val</i></span>. </li><li> The query format is "<span class="tex-span">1</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>k</i></span>". In reply to this query you should print the maximum sum of at most <span class="tex-span"><i>k</i></span> non-intersecting subsegments of sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span>. Formally, you should choose at most <span class="tex-span"><i>k</i></span> pairs of integers <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>), (<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>), ..., (<i>x</i><sub class="lower-index"><i>t</i></sub>, <i>y</i><sub class="lower-index"><i>t</i></sub>)</span> <span class="tex-span">(<i>l</i> ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ <i>y</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>t</i></sub> ≤ <i>y</i><sub class="lower-index"><i>t</i></sub> ≤ <i>r</i>;&nbsp;<i>t</i> ≤ <i>k</i>)</span> such that the sum <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index">1</sub></sub> + <i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index">1</sub> + 1</sub> + ... + <i>a</i><sub class="lower-index"><i>y</i><sub class="lower-index">1</sub></sub> + <i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index">2</sub></sub> + <i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index">2</sub> + 1</sub> + ... + <i>a</i><sub class="lower-index"><i>y</i><sub class="lower-index">2</sub></sub> + ... + <i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>t</i></sub></sub> + <i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>t</i></sub> + 1</sub> + ... + <i>a</i><sub class="lower-index"><i>y</i><sub class="lower-index"><i>t</i></sub></sub></span> is as large as possible. Note that you should choose at most <span class="tex-span"><i>k</i></span> subsegments. Particularly, you can choose 0 subsegments. In this case the described sum considered equal to zero. </li></ul></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, showing how many numbers the sequence has. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 500)</span>. </p><p>The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. The next <span class="tex-span"><i>m</i></span> lines contain the queries in the format, given in the statement.</p><p>All changing queries fit into limits: <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">|<i>val</i>| ≤ 500</span>.</p><p>All queries to count the maximum sum of at most <span class="tex-span"><i>k</i></span> non-intersecting subsegments fit into limits: <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 20</span>. It is guaranteed that the number of the queries to count the maximum sum of at most <span class="tex-span"><i>k</i></span> non-intersecting subsegments doesn't exceed <span class="tex-span">10000</span>.</p></div><div class="output-specification"><p>For each query to count the maximum sum of at most <span class="tex-span"><i>k</i></span> non-intersecting subsegments print the reply — the maximum sum. Print the answers to the queries in the order, in which the queries follow in the input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, showing how many numbers the sequence has. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 500)</span>. </p><p>The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. The next <span class="tex-span"><i>m</i></span> lines contain the queries in the format, given in the statement.</p><p>All changing queries fit into limits: <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">|<i>val</i>| ≤ 500</span>.</p><p>All queries to count the maximum sum of at most <span class="tex-span"><i>k</i></span> non-intersecting subsegments fit into limits: <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 20</span>. It is guaranteed that the number of the queries to count the maximum sum of at most <span class="tex-span"><i>k</i></span> non-intersecting subsegments doesn't exceed <span class="tex-span">10000</span>.</p>

## Output

<p>For each query to count the maximum sum of at most <span class="tex-span"><i>k</i></span> non-intersecting subsegments print the reply — the maximum sum. Print the answers to the queries in the order, in which the queries follow in the input.</p>





```input1
9
9 -8 9 -1 -1 -1 9 -8 9
3
1 1 9 1
1 1 9 2
1 4 6 3

```




```input2
15
-4 8 -3 -10 10 4 -7 -7 0 -6 3 8 -10 7 2
15
1 3 9 2
1 6 12 1
0 6 5
0 10 -7
1 4 9 1
1 7 9 1
0 10 -3
1 4 10 2
1 3 13 2
1 4 11 2
0 15 -9
0 13 -9
0 11 -10
1 5 14 2
1 6 12 1

```




```output1
17
25
0

```




```output2
14
11
15
0
15
26
18
23
8

```



## Note

<p>In the first query of the first example you can select a single pair <span class="tex-span">(1, 9)</span>. So the described sum will be 17.</p><p>Look at the second query of the first example. How to choose two subsegments? (1, 3) and (7, 9)? Definitely not, the sum we could get from (1, 3) and (7, 9) is 20, against the optimal configuration (1, 7) and (9, 9) with 25.</p><p>The answer to the third query is 0, we prefer select nothing if all of the numbers in the given interval are negative.</p>
