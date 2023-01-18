## Description

<div><p>Alice and Bob love playing one-dimensional battle ships. They play on the field in the form of a line consisting of <span class="tex-span"><i>n</i></span> square cells (that is, on a <span class="tex-span">1 × <i>n</i></span> table).</p><p>At the beginning of the game Alice puts <span class="tex-span"><i>k</i></span> ships on the field without telling their positions to Bob. Each ship looks as a <span class="tex-span">1 × <i>a</i></span> rectangle (that is, it occupies a sequence of <span class="tex-span"><i>a</i></span> consecutive squares of the field). The ships cannot intersect and even touch each other.</p><p>After that Bob makes a sequence of "shots". He names cells of the field and Alice either says that the cell is empty ("miss"), or that the cell belongs to some ship ("hit").</p><p>But here's the problem! Alice like to cheat. May be that is why she responds to each Bob's move with a "miss". </p><p>Help Bob catch Alice cheating — find Bob's first move, such that after it you can be sure that Alice cheated.</p></div><div class="input-specification"><p>The first line of the input contains three integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i>, <i>a</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the size of the field, the number of the ships and the size of each ship. It is guaranteed that the <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>a</i></span> are such that you can put <span class="tex-span"><i>k</i></span> ships of size <span class="tex-span"><i>a</i></span> on the field, so that no two ships intersect or touch each other.</p><p>The second line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>) — the number of Bob's moves.</p><p>The third line contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the number of the cell where Bob made the <span class="tex-span"><i>i</i></span>-th shot. The cells are numbered from left to right from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the number of such Bob's first move, after which you can be sure that Alice lied. Bob's moves are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order the were made. If the sought move doesn't exist, then print "<span class="tex-font-style-tt">-1</span>".</p></div>

## Input

<p>The first line of the input contains three integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i>, <i>a</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the size of the field, the number of the ships and the size of each ship. It is guaranteed that the <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>a</i></span> are such that you can put <span class="tex-span"><i>k</i></span> ships of size <span class="tex-span"><i>a</i></span> on the field, so that no two ships intersect or touch each other.</p><p>The second line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>) — the number of Bob's moves.</p><p>The third line contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the number of the cell where Bob made the <span class="tex-span"><i>i</i></span>-th shot. The cells are numbered from left to right from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print a single integer — the number of such Bob's first move, after which you can be sure that Alice lied. Bob's moves are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order the were made. If the sought move doesn't exist, then print "<span class="tex-font-style-tt">-1</span>".</p>





```input1
11 3 3
5
4 8 6 1 11

```




```input2
5 1 3
2
1 5

```




```input3
5 1 3
1
3

```




```output1
3

```




```output2
-1

```




```output3
1

```


