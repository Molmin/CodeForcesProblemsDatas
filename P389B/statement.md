## Description

<div><p>Fox Ciel has a board with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns. So, the board consists of <span class="tex-span"><i>n</i> × <i>n</i></span> cells. Each cell contains either a symbol '<span class="tex-font-style-tt">.</span>', or a symbol '<span class="tex-font-style-tt">#</span>'.</p><p>A cross on the board is a connected set of exactly five cells of the board that looks like a cross. The picture below shows how it looks.</p><center><img class="tex-graphics" src="file://NvAEwOTR.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Ciel wants to draw several (may be zero) crosses on the board. Each cross must cover exactly five cells with symbols '<span class="tex-font-style-tt">#</span>', and any cell with symbol '<span class="tex-font-style-tt">#</span>' must belong to some cross. No two crosses can share a cell.</p><p>Please, tell Ciel if she can draw the crosses in the described way.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — the size of the board.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines describes one row of the board. The <span class="tex-span"><i>i</i></span>-th line describes the <span class="tex-span"><i>i</i></span>-th row of the board and consists of <span class="tex-span"><i>n</i></span> characters. Each character is either a symbol '<span class="tex-font-style-tt">.</span>', or a symbol '<span class="tex-font-style-tt">#</span>'.</p></div><div class="output-specification"><p>Output a single line with "<span class="tex-font-style-tt">YES</span>" if Ciel can draw the crosses in the described way. Otherwise output a single line with "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — the size of the board.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines describes one row of the board. The <span class="tex-span"><i>i</i></span>-th line describes the <span class="tex-span"><i>i</i></span>-th row of the board and consists of <span class="tex-span"><i>n</i></span> characters. Each character is either a symbol '<span class="tex-font-style-tt">.</span>', or a symbol '<span class="tex-font-style-tt">#</span>'.</p>

## Output

<p>Output a single line with "<span class="tex-font-style-tt">YES</span>" if Ciel can draw the crosses in the described way. Otherwise output a single line with "<span class="tex-font-style-tt">NO</span>".</p>





```input1
5
.#...
####.
.####
...#.
.....

```




```input2
4
####
####
####
####

```




```input3
6
.#....
####..
.####.
.#.##.
######
.#..#.

```




```input4
6
.#..#.
######
.####.
.####.
######
.#..#.

```




```input5
3
...
...
...

```




```output1
YES

```




```output2
NO

```




```output3
YES

```




```output4
NO

```




```output5
YES

```



## Note

<p>In example 1, you can draw two crosses. The picture below shows what they look like.</p><center><img class="tex-graphics" src="file://WOIndDq5.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In example 2, the board contains 16 cells with '<span class="tex-font-style-tt">#</span>', but each cross contains 5. Since 16 is not a multiple of 5, so it's impossible to cover all.</p>
