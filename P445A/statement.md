## Description

<div><p><span class="tex-font-style-it">DZY loves chessboard, and he enjoys playing with it.</span></p><p>He has a chessboard of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Some cells of the chessboard are bad, others are good. For every good cell, DZY wants to put a chessman on it. Each chessman is either white or black. After putting all chessmen, DZY wants that no two chessmen with the same color are on two adjacent cells. Two cells are adjacent if and only if they share a common edge.</p><p>You task is to find any suitable placement of chessmen on the given chessboard.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string of <span class="tex-span"><i>m</i></span> characters: the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th string is either "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">-</span>". A "<span class="tex-font-style-tt">.</span>" means that the corresponding cell (in the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column) is good, while a "<span class="tex-font-style-tt">-</span>" means it is bad.</p></div><div class="output-specification"><p>Output must contain <span class="tex-span"><i>n</i></span> lines, each line must contain a string of <span class="tex-span"><i>m</i></span> characters. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th string should be either "<span class="tex-font-style-tt">W</span>", "<span class="tex-font-style-tt">B</span>" or "<span class="tex-font-style-tt">-</span>". Character "<span class="tex-font-style-tt">W</span>" means the chessman on the cell is white, "<span class="tex-font-style-tt">B</span>" means it is black, "<span class="tex-font-style-tt">-</span>" means the cell is a bad cell.</p><p>If multiple answers exist, print any of them. It is guaranteed that at least one answer exists.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string of <span class="tex-span"><i>m</i></span> characters: the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th string is either "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">-</span>". A "<span class="tex-font-style-tt">.</span>" means that the corresponding cell (in the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column) is good, while a "<span class="tex-font-style-tt">-</span>" means it is bad.</p>

## Output

<p>Output must contain <span class="tex-span"><i>n</i></span> lines, each line must contain a string of <span class="tex-span"><i>m</i></span> characters. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th string should be either "<span class="tex-font-style-tt">W</span>", "<span class="tex-font-style-tt">B</span>" or "<span class="tex-font-style-tt">-</span>". Character "<span class="tex-font-style-tt">W</span>" means the chessman on the cell is white, "<span class="tex-font-style-tt">B</span>" means it is black, "<span class="tex-font-style-tt">-</span>" means the cell is a bad cell.</p><p>If multiple answers exist, print any of them. It is guaranteed that at least one answer exists.</p>





```input1
1 1
.

```




```input2
2 2
..
..

```




```input3
3 3
.-.
---
--.
```




```output1
B

```




```output2
BW
WB

```




```output3
B-B
---
--B
```



## Note

<p>In the first sample, DZY puts a single black chessman. Of course putting a white one is also OK.</p><p>In the second sample, all <span class="tex-span">4</span> cells are good. No two same chessmen share an edge in the sample output.</p><p>In the third sample, no good cells are adjacent. So you can just put <span class="tex-span">3</span> chessmen, no matter what their colors are.</p>
