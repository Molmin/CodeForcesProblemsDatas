## Description

<div><p>Fox Ciel has a board with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns, there is one integer in each cell.</p><p>It's known that <span class="tex-span"><i>n</i></span> is an odd number, so let's introduce <img align="middle" class="tex-formula" src="file://QdU3l2kc.png" style="max-width: 100.0%;max-height: 100.0%;">. Fox Ciel can do the following operation many times: she choose a sub-board with size <span class="tex-span"><i>x</i></span> rows and <span class="tex-span"><i>x</i></span> columns, then all numbers in it will be multiplied by -1.</p><p>Return the maximal sum of numbers in the board that she can get by these operations.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span>, (<span class="tex-span">1 ≤ <i>n</i> ≤ 33</span>, and <span class="tex-span"><i>n</i></span> is an odd integer) — the size of the board.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers — the numbers in the board. Each number doesn't exceed <span class="tex-span">1000</span> by its absolute value.</p></div><div class="output-specification"><p>Output a single integer: the maximal sum of numbers in the board that can be accomplished.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span>, (<span class="tex-span">1 ≤ <i>n</i> ≤ 33</span>, and <span class="tex-span"><i>n</i></span> is an odd integer) — the size of the board.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers — the numbers in the board. Each number doesn't exceed <span class="tex-span">1000</span> by its absolute value.</p>

## Output

<p>Output a single integer: the maximal sum of numbers in the board that can be accomplished.</p>





```input1
3
-1 -1 1
-1 1 -1
1 -1 -1

```




```input2
5
-2 0 0 0 -2
0 -2 0 -2 0
0 0 -2 0 0
0 -2 0 -2 0
-2 0 0 0 -2

```




```output1
9

```




```output2
18

```



## Note

<p>In the first test, we can apply this operation twice: first on the top left <span class="tex-span">2 × 2</span> sub-board, then on the bottom right <span class="tex-span">2 × 2</span> sub-board. Then all numbers will become positive.</p><p><img class="tex-graphics" src="file://YBbs2ZUM.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
