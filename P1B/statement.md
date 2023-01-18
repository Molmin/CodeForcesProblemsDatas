## Description

<div><p>In the popular spreadsheets systems (for example, in Excel) the following numeration of columns is used. The first column has number A, the second — number B, etc. till column 26 that is marked by Z. Then there are two-letter numbers: column 27 has number AA, 28 — AB, column 52 is marked by AZ. After ZZ there follow three-letter numbers, etc.</p><p>The rows are marked by integer numbers starting with 1. The cell name is the concatenation of the column and the row numbers. For example, BC23 is the name for the cell that is in column 55, row 23. </p><p>Sometimes another numeration system is used: RXCY, where X and Y are integer numbers, showing the column and the row numbers respectfully. For instance, R23C55 is the cell from the previous example.</p><p>Your task is to write a program that reads the given sequence of cell coordinates and produce each item written according to the rules of another numeration system.</p></div><div class="input-specification"><p>The first line of the input contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of coordinates in the test. Then there follow <span class="tex-span"><i>n</i></span> lines, each of them contains coordinates. All the coordinates are correct, there are no cells with the column and/or the row numbers larger than <span class="tex-span">10<sup class="upper-index">6</sup></span> .</p></div><div class="output-specification"><p>Write <span class="tex-span"><i>n</i></span> lines, each line should contain a cell coordinates in the other numeration system.</p></div>

## Input

<p>The first line of the input contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of coordinates in the test. Then there follow <span class="tex-span"><i>n</i></span> lines, each of them contains coordinates. All the coordinates are correct, there are no cells with the column and/or the row numbers larger than <span class="tex-span">10<sup class="upper-index">6</sup></span> .</p>

## Output

<p>Write <span class="tex-span"><i>n</i></span> lines, each line should contain a cell coordinates in the other numeration system.</p>





```input1
2
R23C55
BC23

```




```output1
BC23
R23C55

```


