## Description

<div><p>A two dimensional array is called a <span class="tex-font-style-underline">bracket</span> array if each grid contains one of the two possible brackets — "(" or ")". A path through the two dimensional array cells is called <span class="tex-font-style-underline">monotonous</span> if any two consecutive cells in the path are side-adjacent and each cell of the path is located below or to the right from the previous one. </p><p>A two dimensional array whose size equals <span class="tex-span"><i>n</i> × <i>m</i></span> is called a <span class="tex-font-style-underline">correct bracket</span> array, if any string formed by writing out the brackets on some monotonous way from cell <span class="tex-span">(1, 1)</span> to cell <span class="tex-span">(<i>n</i>, <i>m</i>)</span> forms a correct bracket sequence. </p><p>Let's define the operation of comparing two correct bracket arrays of equal size (<span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>) like that. Let's consider a given two dimensional array of priorities (<span class="tex-span"><i>c</i></span>) — a two dimensional array of same size, containing different integers from <span class="tex-span">1</span> to <span class="tex-span"><i>nm</i></span>. Let's find such position <span class="tex-span">(<i>i</i>, <i>j</i>)</span> in the two dimensional array, that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. If there are several such positions, let's choose the one where number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is minimum. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = </span>"(", then <span class="tex-span"><i>a</i> &lt; <i>b</i></span>, otherwise <span class="tex-span"><i>a</i> &gt; <i>b</i></span>. If the position <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is not found, then the arrays are considered equal.</p><p>Your task is to find a <span class="tex-span"><i>k</i></span>-th two dimensional correct bracket array. It is guaranteed that for the given sizes of <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> there will be no less than <span class="tex-span"><i>k</i></span> two dimensional correct bracket arrays.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> — the sizes of the array and the number of the sought correct bracket array (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>). Then an array of priorities is given, <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> numbers, number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> shows the priority of character <span class="tex-span"><i>j</i></span> in line <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>nm</i></span>, all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> are different).</p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specificator.</p></div><div class="output-specification"><p>Print the <span class="tex-span"><i>k</i></span>-th two dimensional correct bracket array.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> — the sizes of the array and the number of the sought correct bracket array (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>). Then an array of priorities is given, <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> numbers, number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> shows the priority of character <span class="tex-span"><i>j</i></span> in line <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>nm</i></span>, all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> are different).</p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specificator.</p>

## Output

<p>Print the <span class="tex-span"><i>k</i></span>-th two dimensional correct bracket array.</p>





```input1
1 2 1
1 2

```




```input2
2 3 1
1 2 3
4 5 6

```




```input3
3 2 2
3 6
1 4
2 5

```




```output1
()

```




```output2
(()
())

```




```output3
()
)(
()

```



## Note

<p>In the first sample exists only one correct two-dimensional bracket array.</p><p>In the second and in the third samples two arrays exist.</p><p>A bracket sequence is called regular if it is possible to obtain correct arithmetic expression by inserting characters «<span class="tex-font-style-tt">+</span>» and «<span class="tex-font-style-tt">1</span>» into this sequence. For example, sequences «<span class="tex-font-style-tt">(())()</span>», «<span class="tex-font-style-tt">()</span>» and «<span class="tex-font-style-tt">(()(()))</span>» are regular, while «<span class="tex-font-style-tt">)(</span>», «<span class="tex-font-style-tt">(()</span>» and «<span class="tex-font-style-tt">(()))(</span>» are not.</p>
