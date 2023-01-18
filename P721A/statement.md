## Description

<div><p>Recently Adaltik discovered japanese crosswords. Japanese crossword is a picture, represented as a table sized <span class="tex-span"><i>a</i> × <i>b</i></span> squares, and each square is colored white or black. There are integers to the left of the rows and to the top of the columns, encrypting the corresponding row or column. The number of integers represents how many groups of black squares there are in corresponding row or column, and the integers themselves represents the number of consecutive black squares in corresponding group (you can find more detailed explanation in Wikipedia <a href="https://en.wikipedia.org/wiki/Japanese_crossword">https://en.wikipedia.org/wiki/Japanese_crossword</a>).</p><p>Adaltik decided that the general case of japanese crossword is too complicated and drew a row consisting of <span class="tex-span"><i>n</i></span> squares (e.g. japanese crossword sized <span class="tex-span">1 × <i>n</i></span>), which he wants to encrypt in the same way as in japanese crossword.</p><center> <img class="tex-graphics" src="file://W53NtGWH.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The example of encrypting of a single row of japanese crossword.</span> </center><p>Help Adaltik find the numbers encrypting the row he drew.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the row. The second line of the input contains a single string consisting of <span class="tex-span"><i>n</i></span> characters '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">W</span>', ('<span class="tex-font-style-tt">B</span>' corresponds to black square, '<span class="tex-font-style-tt">W</span>'&nbsp;— to white square in the row that Adaltik drew).</p></div><div class="output-specification"><p>The first line should contain a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of integers encrypting the row, e.g. the number of groups of black squares in the row.</p><p>The second line should contain <span class="tex-span"><i>k</i></span> integers, encrypting the row, e.g. corresponding to sizes of groups of consecutive black squares in the order from left to right.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the row. The second line of the input contains a single string consisting of <span class="tex-span"><i>n</i></span> characters '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">W</span>', ('<span class="tex-font-style-tt">B</span>' corresponds to black square, '<span class="tex-font-style-tt">W</span>'&nbsp;— to white square in the row that Adaltik drew).</p>

## Output

<p>The first line should contain a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of integers encrypting the row, e.g. the number of groups of black squares in the row.</p><p>The second line should contain <span class="tex-span"><i>k</i></span> integers, encrypting the row, e.g. corresponding to sizes of groups of consecutive black squares in the order from left to right.</p>





```input1
3
BBW

```




```input2
5
BWBWB

```




```input3
4
WWWW

```




```input4
4
BBBB

```




```input5
13
WBBBBWWBWBBBW

```




```output1
1
2
```




```output2
3
1 1 1
```




```output3
0

```




```output4
1
4
```




```output5
3
4 1 3
```



## Note

<p>The last sample case correspond to the picture in the statement.</p>
