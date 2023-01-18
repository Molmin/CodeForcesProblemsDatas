## Description

<div><p>John Doe has four arrays: <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span>, and <span class="tex-span"><i>p</i></span>. Each array consists of <span class="tex-span"><i>n</i></span> integers. Elements of all arrays are indexed starting from <span class="tex-span">1</span>. Array <span class="tex-span"><i>p</i></span> is a permutation of integers <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>John invented a game for his friends and himself. Initially a player is given array <span class="tex-span"><i>a</i></span>. The player must consecutively execute exactly <span class="tex-span"><i>u</i></span> operations on <span class="tex-span"><i>a</i></span>. You are permitted to execute the following operations:</p><ul> <li> Operation 1: For each <img align="middle" class="tex-formula" src="file://dxgymhSq.png" style="max-width: 100.0%;max-height: 100.0%;"> change <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> into <img align="middle" class="tex-formula" src="file://XdVtu40J.png" style="max-width: 100.0%;max-height: 100.0%;">. Expression <img align="middle" class="tex-formula" src="file://pCp64j8L.png" style="max-width: 100.0%;max-height: 100.0%;"> means applying the operation of a bitwise xor to numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. The given operation exists in all modern programming languages, for example, in language <span class="tex-font-style-it">C++</span> and <span class="tex-font-style-it">Java</span> it is marked as "^", in <span class="tex-font-style-it">Pascal</span> — as "xor". </li><li> Operation 2: For each <img align="middle" class="tex-formula" src="file://NJLbU4Qw.png" style="max-width: 100.0%;max-height: 100.0%;"> change <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> into <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub> + <i>r</i></span>. When this operation is executed, all changes are made at the same time. </li></ul><p>After all <span class="tex-span"><i>u</i></span> operations are applied, the number of points the player gets is determined by the formula <img align="middle" class="tex-formula" src="file://1Q9RYF2F.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>John wants to find out what maximum number of points a player can win in his game. Help him.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>u</i> ≤ 30</span>, <span class="tex-span">0 ≤ <i>r</i> ≤ 100</span>) — the number of elements in each array, the number of operations and the number that describes one of the operations. </p><p>Each of the next four lines contains <span class="tex-span"><i>n</i></span> space-separated integers — arrays <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>p</i></span>. The first line has array <span class="tex-span"><i>a</i></span>, the second line has array <span class="tex-span"><i>b</i></span>, the third line has array <span class="tex-span"><i>k</i></span> and the fourth one has array <span class="tex-span"><i>p</i></span>. </p><p>It is guaranteed that elements of arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are positive and do not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>, elements of array <span class="tex-span"><i>k</i></span> do not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> in the absolute value <span class="tex-span">(|<i>k</i>| ≤ 10<sup class="upper-index">4</sup>)</span> and <span class="tex-span"><i>p</i></span> is a permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>On a single line print number <span class="tex-span"><i>s</i></span> — the maximum number of points that a player can win in John's game.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>u</i> ≤ 30</span>, <span class="tex-span">0 ≤ <i>r</i> ≤ 100</span>) — the number of elements in each array, the number of operations and the number that describes one of the operations. </p><p>Each of the next four lines contains <span class="tex-span"><i>n</i></span> space-separated integers — arrays <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>p</i></span>. The first line has array <span class="tex-span"><i>a</i></span>, the second line has array <span class="tex-span"><i>b</i></span>, the third line has array <span class="tex-span"><i>k</i></span> and the fourth one has array <span class="tex-span"><i>p</i></span>. </p><p>It is guaranteed that elements of arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are positive and do not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>, elements of array <span class="tex-span"><i>k</i></span> do not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> in the absolute value <span class="tex-span">(|<i>k</i>| ≤ 10<sup class="upper-index">4</sup>)</span> and <span class="tex-span"><i>p</i></span> is a permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>On a single line print number <span class="tex-span"><i>s</i></span> — the maximum number of points that a player can win in John's game.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p>





```input1
3 2 1
7 7 7
8 8 8
1 2 3
1 3 2

```




```input2
2 1 0
1 1
1 1
1 -1
1 2

```




```output1
96

```




```output2
0

```



## Note

<p>In the first sample you should first apply the operation of the first type, then the operation of the second type.</p>
