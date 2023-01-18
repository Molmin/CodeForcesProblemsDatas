## Description

<div><p>Vasya has the square chessboard of size <span class="tex-span"><i>n</i> × <i>n</i></span> and <span class="tex-span"><i>m</i></span> rooks. Initially the chessboard is empty. Vasya will consequently put the rooks on the board one after another.</p><p>The cell of the field is under rook's attack, if there is at least one rook located in the same row or in the same column with this cell. If there is a rook located in the cell, this cell is also under attack.</p><p>You are given the positions of the board where Vasya will put rooks. For each rook you have to determine the number of cells which are <span class="tex-font-style-bf">not under attack</span> after Vasya puts it on the board.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>min</i>(100 000, <i>n</i><sup class="upper-index">2</sup>)</span>)&nbsp;— the size of the board and the number of rooks. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the number of the row and the number of the column where Vasya will put the <span class="tex-span"><i>i</i></span>-th rook. Vasya puts rooks on the board in the order they appear in the input. It is guaranteed that any cell will contain no more than one rook.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integer, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of cells that are not under attack after first <span class="tex-span"><i>i</i></span> rooks are put.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>min</i>(100 000, <i>n</i><sup class="upper-index">2</sup>)</span>)&nbsp;— the size of the board and the number of rooks. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the number of the row and the number of the column where Vasya will put the <span class="tex-span"><i>i</i></span>-th rook. Vasya puts rooks on the board in the order they appear in the input. It is guaranteed that any cell will contain no more than one rook.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integer, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of cells that are not under attack after first <span class="tex-span"><i>i</i></span> rooks are put.</p>





```input1
3 3
1 1
3 1
2 2

```




```input2
5 2
1 5
5 1

```




```input3
100000 1
300 400

```




```output1
4 2 0 

```




```output2
16 9 

```




```output3
9999800001 

```



## Note

<p>On the picture below show the state of the board after put each of the three rooks. The cells which painted with grey color is not under the attack.</p><center> <img class="tex-graphics" src="file://aMxJyIRy.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
