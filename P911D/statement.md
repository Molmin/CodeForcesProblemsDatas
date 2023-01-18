## Description

<div><p>A permutation of size <span class="tex-span"><i>n</i></span> is an array of size <span class="tex-span"><i>n</i></span> such that each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs exactly once in this array. An inversion in a permutation <span class="tex-span"><i>p</i></span> is a pair of indices <span class="tex-span">(<i>i</i>, <i>j</i>)</span> such that <span class="tex-span"><i>i</i> &gt; <i>j</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>j</i></sub></span>. For example, a permutation <span class="tex-span">[4, 1, 3, 2]</span> contains <span class="tex-span">4</span> inversions: <span class="tex-span">(2, 1)</span>, <span class="tex-span">(3, 1)</span>, <span class="tex-span">(4, 1)</span>, <span class="tex-span">(4, 3)</span>.</p><p>You are given a permutation <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> queries to it. Each query is represented by two indices <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> denoting that you have to reverse the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> of the permutation. For example, if <span class="tex-span"><i>a</i> = [1, 2, 3, 4]</span> and a query <span class="tex-span"><i>l</i> = 2</span>, <span class="tex-span"><i>r</i> = 4</span> is applied, then the resulting permutation is <span class="tex-span">[1, 4, 3, 2]</span>.</p><p>After each query you have to determine whether the number of inversions is odd or even.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1500</span>) — the size of the permutation. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the elements of the permutation. These integers are pairwise distinct.</p><p>The third line contains one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of queries to process.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) denoting that <span class="tex-span"><i>i</i></span>-th query is to reverse a segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> of the permutation. All queries are performed one after another.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. <span class="tex-span"><i>i</i></span>-th of them must be equal to <span class="tex-font-style-tt">odd</span> if the number of inversions in the permutation after <span class="tex-span"><i>i</i></span>-th query is odd, and <span class="tex-font-style-tt">even</span> otherwise.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1500</span>) — the size of the permutation. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the elements of the permutation. These integers are pairwise distinct.</p><p>The third line contains one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of queries to process.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) denoting that <span class="tex-span"><i>i</i></span>-th query is to reverse a segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> of the permutation. All queries are performed one after another.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. <span class="tex-span"><i>i</i></span>-th of them must be equal to <span class="tex-font-style-tt">odd</span> if the number of inversions in the permutation after <span class="tex-span"><i>i</i></span>-th query is odd, and <span class="tex-font-style-tt">even</span> otherwise.</p>





```input1
3
1 2 3
2
1 2
2 3

```




```input2
4
1 2 4 3
4
1 1
1 4
1 4
2 3

```




```output1
odd
even

```




```output2
odd
odd
odd
even

```



## Note

<p>The first example:</p><ol> <li> after the first query <span class="tex-span"><i>a</i> = [2, 1, 3]</span>, inversion: <span class="tex-span">(2, 1)</span>; </li><li> after the second query <span class="tex-span"><i>a</i> = [2, 3, 1]</span>, inversions: <span class="tex-span">(3, 1)</span>, <span class="tex-span">(3, 2)</span>. </li></ol><p>The second example:</p><ol> <li> <span class="tex-span"><i>a</i> = [1, 2, 4, 3]</span>, inversion: <span class="tex-span">(4, 3)</span>; </li><li> <span class="tex-span"><i>a</i> = [3, 4, 2, 1]</span>, inversions: <span class="tex-span">(3, 1)</span>, <span class="tex-span">(4, 1)</span>, <span class="tex-span">(3, 2)</span>, <span class="tex-span">(4, 2)</span>, <span class="tex-span">(4, 3)</span>; </li><li> <span class="tex-span"><i>a</i> = [1, 2, 4, 3]</span>, inversion: <span class="tex-span">(4, 3)</span>; </li><li> <span class="tex-span"><i>a</i> = [1, 4, 2, 3]</span>, inversions: <span class="tex-span">(3, 2)</span>, <span class="tex-span">(4, 2)</span>. </li></ol>
