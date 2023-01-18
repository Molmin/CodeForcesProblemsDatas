## Description

<div><p>There are many interesting tasks on domino tilings. For example, an interesting fact is known. Let us take a standard chessboard (<span class="tex-span">8 × 8</span>) and cut exactly two squares out of it. It turns out that the resulting board can always be tiled using dominoes <span class="tex-span">1 × 2</span>, if the two cut out squares are of the same color, otherwise it is impossible. </p><p>Petya grew bored with dominoes, that's why he took a chessboard (not necessarily <span class="tex-span">8 × 8</span>), cut some squares out of it and tries to tile it using triminoes. Triminoes are reactangles <span class="tex-span">1 × 3</span> (or <span class="tex-span">3 × 1</span>, because triminoes can be rotated freely), also the two extreme squares of a trimino are necessarily white and the square in the middle is black. The triminoes are allowed to put on the chessboard so that their squares matched the colors of the uncut squares of the chessboard, and also the colors must match: the black squares must be matched with the black ones only and the white ones — with the white squares. The triminoes must not protrude above the chessboard or overlap each other. All the uncut squares of the board must be covered with triminoes. </p><p>Help Petya find out if it is possible to tile his board using triminos in the described way and print one of the variants of tiling.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the board size. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> symbols each and represent the board description. If some position contains ".", then the square in this position has been cut out. Symbol "w" stands for a white square, "b" stands for a black square. It is guaranteed that through adding the cut squares can result in a correct chessboard (i.e. with alternating black and white squares), thought, perhaps, of a non-standard size.</p></div><div class="output-specification"><p>If at least one correct tiling exists, in the first line print "YES" (without quotes), and then — the tiling description. The description must contain <span class="tex-span"><i>n</i></span> lines, <span class="tex-span"><i>m</i></span> symbols in each. The cut out squares, as well as in the input data, are marked by ".". To denote triminoes symbols "a", "b", "c", "d" can be used, and all the three squares of each trimino must be denoted by the same symbol. If two triminoes share a side, than they must be denoted by different symbols. Two triminoes not sharing a common side can be denoted by one and the same symbol (c.f. sample).</p><p>If there are multiple correct ways of tiling, it is allowed to print any. If it is impossible to tile the board using triminoes or the correct tiling, for which four symbols "a", "b", "c", "d" would be enough, doesn't exist, print "NO" (without quotes) in the first line.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the board size. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> symbols each and represent the board description. If some position contains ".", then the square in this position has been cut out. Symbol "w" stands for a white square, "b" stands for a black square. It is guaranteed that through adding the cut squares can result in a correct chessboard (i.e. with alternating black and white squares), thought, perhaps, of a non-standard size.</p>

## Output

<p>If at least one correct tiling exists, in the first line print "YES" (without quotes), and then — the tiling description. The description must contain <span class="tex-span"><i>n</i></span> lines, <span class="tex-span"><i>m</i></span> symbols in each. The cut out squares, as well as in the input data, are marked by ".". To denote triminoes symbols "a", "b", "c", "d" can be used, and all the three squares of each trimino must be denoted by the same symbol. If two triminoes share a side, than they must be denoted by different symbols. Two triminoes not sharing a common side can be denoted by one and the same symbol (c.f. sample).</p><p>If there are multiple correct ways of tiling, it is allowed to print any. If it is impossible to tile the board using triminoes or the correct tiling, for which four symbols "a", "b", "c", "d" would be enough, doesn't exist, print "NO" (without quotes) in the first line.</p>





```input1
6 10
.w.wbw.wbw
wbwbw.w.w.
bw.wbwbwbw
w.wbw.wbwb
...wbw.w.w
..wbw.wbw.

```




```input2
2 2
wb
bw

```




```input3
1 3
wbw

```




```input4
1 3
...

```




```output1
YES
.a.aaa.ccc
baccc.c.a.
ba.dddcbab
b.aaa.cbab
...bbb.b.b
..ccc.ddd.
```




```output2
NO

```




```output3
YES
bbb

```




```output4
YES
...

```


