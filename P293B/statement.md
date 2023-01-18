## Description

<div><p>You have a rectangular <span class="tex-span"><i>n</i> × <i>m</i></span>-cell board. Some cells are already painted some of <span class="tex-span"><i>k</i></span> colors. You need to paint each uncolored cell one of the <span class="tex-span"><i>k</i></span> colors so that any path from the upper left square to the lower right one doesn't contain any two cells of the same color. The path can go only along side-adjacent cells and can only go down or right.</p><p>Print the number of possible paintings modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000, 1 ≤ <i>k</i> ≤ 10)</span>. The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> integers each — the board. The first of them contains <span class="tex-span"><i>m</i></span> uppermost cells of the board from the left to the right and the second one contains <span class="tex-span"><i>m</i></span> cells from the second uppermost row and so on. If a number in a line equals 0, then the corresponding cell isn't painted. Otherwise, this number represents the initial color of the board cell — an integer from 1 to <span class="tex-span"><i>k</i></span>.</p><p>Consider all colors numbered from 1 to <span class="tex-span"><i>k</i></span> in some manner.</p></div><div class="output-specification"><p>Print the number of possible paintings modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000, 1 ≤ <i>k</i> ≤ 10)</span>. The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> integers each — the board. The first of them contains <span class="tex-span"><i>m</i></span> uppermost cells of the board from the left to the right and the second one contains <span class="tex-span"><i>m</i></span> cells from the second uppermost row and so on. If a number in a line equals 0, then the corresponding cell isn't painted. Otherwise, this number represents the initial color of the board cell — an integer from 1 to <span class="tex-span"><i>k</i></span>.</p><p>Consider all colors numbered from 1 to <span class="tex-span"><i>k</i></span> in some manner.</p>

## Output

<p>Print the number of possible paintings modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2 2 4
0 0
0 0

```




```input2
2 2 4
1 2
2 1

```




```input3
5 6 10
0 0 0 0 0 0
0 0 0 0 0 0
0 0 0 0 0 0
0 0 0 0 0 0
0 0 0 0 0 0

```




```input4
2 6 10
1 2 3 4 5 6
0 0 0 0 0 0

```




```output1
48

```




```output2
0

```




```output3
3628800

```




```output4
4096

```


