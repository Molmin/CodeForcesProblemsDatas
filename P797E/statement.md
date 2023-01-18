## Description

<div><p><span class="tex-span"><i>a</i></span> is an array of <span class="tex-span"><i>n</i></span> positive integers, all of which are not greater than <span class="tex-span"><i>n</i></span>.</p><p>You have to process <span class="tex-span"><i>q</i></span> queries to this array. Each query is represented by two numbers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span>. Several operations are performed in each query; each operation changes <span class="tex-span"><i>p</i></span> to <span class="tex-span"><i>p</i> + <i>a</i><sub class="lower-index"><i>p</i></sub> + <i>k</i></span>. There operations are applied until <span class="tex-span"><i>p</i></span> becomes greater than <span class="tex-span"><i>n</i></span>. The answer to the query is the number of performed operations.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100000)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers — elements of <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> for each <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>).</p><p>The third line containts one integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 100000)</span>.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. Each line contains the values of <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span> for corresponding query <span class="tex-span">(1 ≤ <i>p</i>, <i>k</i> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> integers, <span class="tex-span"><i>i</i></span>th integer must be equal to the answer to <span class="tex-span"><i>i</i></span>th query.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100000)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers — elements of <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> for each <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>).</p><p>The third line containts one integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 100000)</span>.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. Each line contains the values of <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span> for corresponding query <span class="tex-span">(1 ≤ <i>p</i>, <i>k</i> ≤ <i>n</i>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> integers, <span class="tex-span"><i>i</i></span>th integer must be equal to the answer to <span class="tex-span"><i>i</i></span>th query.</p>





```input1
3
1 1 1
3
1 1
2 1
3 1

```




```output1
2
1
1

```



## Note

<p>Consider first example:</p><p>In first query after first operation <span class="tex-span"><i>p</i> = 3</span>, after second operation <span class="tex-span"><i>p</i> = 5</span>.</p><p>In next two queries <span class="tex-span"><i>p</i></span> is greater than <span class="tex-span"><i>n</i></span> after the first operation.</p>
