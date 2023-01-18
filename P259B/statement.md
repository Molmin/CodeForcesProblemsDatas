## Description

<div><p>Little Elephant loves magic squares very much.</p><p>A <span class="tex-font-style-it">magic square</span> is a <span class="tex-span">3 × 3</span> table, each cell contains some positive integer. At that the sums of integers in all rows, columns and diagonals of the table are equal. The figure below shows the magic square, the sum of integers in all its rows, columns and diagonals equals 15.</p><center> <img class="tex-graphics" src="file://L1uVH9dA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The Little Elephant remembered one magic square. He started writing this square on a piece of paper, but as he wrote, he forgot all three elements of the main diagonal of the magic square. Fortunately, the Little Elephant clearly remembered that all elements of the magic square did not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. </p><p>Help the Little Elephant, restore the original magic square, given the Elephant's notes.</p></div><div class="input-specification"><p>The first three lines of the input contain the Little Elephant's notes. The first line contains elements of the first row of the magic square. The second line contains the elements of the second row, the third line is for the third row. The main diagonal elements that have been forgotten by the Elephant are represented by zeroes.</p><p>It is guaranteed that the notes contain exactly three zeroes and they are all located on the main diagonal. It is guaranteed that all positive numbers in the table do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print three lines, in each line print three integers — the Little Elephant's magic square. If there are multiple magic squares, you are allowed to print any of them. Note that all numbers you print must be positive and not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that there exists at least one magic square that meets the conditions.</p></div>

## Input

<p>The first three lines of the input contain the Little Elephant's notes. The first line contains elements of the first row of the magic square. The second line contains the elements of the second row, the third line is for the third row. The main diagonal elements that have been forgotten by the Elephant are represented by zeroes.</p><p>It is guaranteed that the notes contain exactly three zeroes and they are all located on the main diagonal. It is guaranteed that all positive numbers in the table do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print three lines, in each line print three integers — the Little Elephant's magic square. If there are multiple magic squares, you are allowed to print any of them. Note that all numbers you print must be positive and not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that there exists at least one magic square that meets the conditions.</p>





```input1
0 1 1
1 0 1
1 1 0

```




```input2
0 3 6
5 0 5
4 7 0

```




```output1
1 1 1
1 1 1
1 1 1

```




```output2
6 3 6
5 5 5
4 7 4

```


