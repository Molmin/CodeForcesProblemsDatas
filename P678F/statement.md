## Description

<div><p>Lena is a programmer. She got a task to solve at work.</p><p>There is an empty set of pairs of integers and <span class="tex-span"><i>n</i></span> queries to process. Each query is one of three types:</p><ol> <li> Add a pair <span class="tex-span">(<i>a</i>, <i>b</i>)</span> to the set. </li><li> Remove a pair added in the query number <span class="tex-span"><i>i</i></span>. All queries are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </li><li> For a given integer <span class="tex-span"><i>q</i></span> find the maximal value <span class="tex-span"><i>x</i>·<i>q</i> + <i>y</i></span> over all pairs <span class="tex-span">(<i>x</i>, <i>y</i>)</span> from the set. </li></ol><p>Help Lena to process the queries.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of queries.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines starts with integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 3</span>) — the type of the query.</p><p>A pair of integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>) follows in the query of the first type.</p><p>An integer <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) follows in the query of the second type. It is guaranteed that <span class="tex-span"><i>i</i></span> is less than the number of the query, the query number <span class="tex-span"><i>i</i></span> has the first type and the pair from the <span class="tex-span"><i>i</i></span>-th query is not already removed.</p><p>An integer <span class="tex-span"><i>q</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>q</i> ≤ 10<sup class="upper-index">9</sup></span>) follows in the query of the third type.</p></div><div class="output-specification"><p>For the queries of the third type print on a separate line the desired maximal value of <span class="tex-span"><i>x</i>·<i>q</i> + <i>y</i></span>.</p><p>If there are no pairs in the set print "<span class="tex-font-style-tt">EMPTY SET</span>".</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of queries.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines starts with integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 3</span>) — the type of the query.</p><p>A pair of integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>) follows in the query of the first type.</p><p>An integer <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) follows in the query of the second type. It is guaranteed that <span class="tex-span"><i>i</i></span> is less than the number of the query, the query number <span class="tex-span"><i>i</i></span> has the first type and the pair from the <span class="tex-span"><i>i</i></span>-th query is not already removed.</p><p>An integer <span class="tex-span"><i>q</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>q</i> ≤ 10<sup class="upper-index">9</sup></span>) follows in the query of the third type.</p>

## Output

<p>For the queries of the third type print on a separate line the desired maximal value of <span class="tex-span"><i>x</i>·<i>q</i> + <i>y</i></span>.</p><p>If there are no pairs in the set print "<span class="tex-font-style-tt">EMPTY SET</span>".</p>





```input1
7
3 1
1 2 3
3 1
1 -1 100
3 1
2 4
3 1

```




```output1
EMPTY SET
5
99
5

```


