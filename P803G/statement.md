## Description

<div><p>You are given an array <span class="tex-span"><i>a</i></span> consisting of positive integers and <span class="tex-span"><i>q</i></span> queries to this array. There are two types of queries: </p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>x</i></span> — for each index <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> set <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>x</i></span>. </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> — find the minimum among such <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span>. </li></ul><p>We decided that this problem is too easy. So the array <span class="tex-span"><i>a</i></span> is given in a compressed form: there is an array <span class="tex-span"><i>b</i></span> consisting of <span class="tex-span"><i>n</i></span> elements and a number <span class="tex-span"><i>k</i></span> in the input, and before all queries <span class="tex-span"><i>a</i></span> is equal to the concatenation of <span class="tex-span"><i>k</i></span> arrays <span class="tex-span"><i>b</i></span> (so the size of <span class="tex-span"><i>a</i></span> is <span class="tex-span"><i>n</i>·<i>k</i></span>).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers — elements of the array <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, each representing a query. Each query is given either as <span class="tex-span">1</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>x</i></span> — set all elements in the segment from <span class="tex-span"><i>l</i></span> till <span class="tex-span"><i>r</i></span> (including borders) to <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>·<i>k</i></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) or as <span class="tex-span">2</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> — find the minimum among all elements in the segment from <span class="tex-span"><i>l</i></span> till <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>·<i>k</i></span>).</p></div><div class="output-specification"><p>For each query of type <span class="tex-span">2</span> print the answer to this query — the minimum on the corresponding segment.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers — elements of the array <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, each representing a query. Each query is given either as <span class="tex-span">1</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>x</i></span> — set all elements in the segment from <span class="tex-span"><i>l</i></span> till <span class="tex-span"><i>r</i></span> (including borders) to <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>·<i>k</i></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) or as <span class="tex-span">2</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> — find the minimum among all elements in the segment from <span class="tex-span"><i>l</i></span> till <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>·<i>k</i></span>).</p>

## Output

<p>For each query of type <span class="tex-span">2</span> print the answer to this query — the minimum on the corresponding segment.</p>





```input1
3 1
1 2 3
3
2 1 3
1 1 2 4
2 1 3

```




```input2
3 2
1 2 3
5
2 4 4
1 4 4 5
2 4 4
1 1 6 1
2 6 6

```




```output1
1
3

```




```output2
1
5
1

```


