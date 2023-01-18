## Description

<div><p>There is a square box <span class="tex-span">6 × 6</span> in size. It contains <span class="tex-span">36</span> chips <span class="tex-span">1 × 1</span> in size. Those chips contain 36 different characters — "<span class="tex-font-style-tt">0</span>"-"<span class="tex-font-style-tt">9</span>" and "<span class="tex-font-style-tt">A</span>"-"<span class="tex-font-style-tt">Z</span>". There is exactly one chip with each character.</p><p>You are allowed to make the following operations: you may choose one of <span class="tex-span">6</span> rows or one of <span class="tex-span">6</span> columns and cyclically shift the chips there to one position to the left or to the right (for the row) or upwards or downwards (for the column). Those operations are allowed to perform several times. </p><p>To solve the puzzle is to shift the chips using the above described operations so that they were written in the increasing order (exactly equal to the right picture). An example of solving the puzzle is shown on a picture below.</p><center> <img class="tex-graphics" src="file://WthId81O.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Write a program that finds the sequence of operations that solves the puzzle. That sequence <span class="tex-font-style-bf">should not necessarily be shortest</span>, but you should not exceed the limit of <span class="tex-span">10000</span> operations. It is guaranteed that the solution always exists.</p></div><div class="input-specification"><p>The input data are represented by 6 lines containing 6 characters each. They are the puzzle's initial position. Those lines contain each character from the string "<span class="tex-font-style-tt">0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ</span>" exactly once.</p></div><div class="output-specification"><p>On the first line print number <span class="tex-span"><i>n</i></span>, which is the number of operations. On the next <span class="tex-span"><i>n</i></span> lines print the sequence of operations one per line. An operation is described by a word consisting of two characters. The first character shows the direction where the row or the column will be shifted. The possible directions are "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" (to the left, to the right correspondingly, we shift a row), "<span class="tex-font-style-tt">U</span>", "<span class="tex-font-style-tt">D</span>" (upwards, downwards correspondingly, we shift a column). The second character is the number of the row (or the column), it is an integer from "<span class="tex-font-style-tt">1</span>" to "<span class="tex-font-style-tt">6</span>". The rows are numbered from the top to the bottom, the columns are numbered from the left to the right.</p><p>The number of operations should not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. If there are several solutions, print any of them.</p></div>

## Input

<p>The input data are represented by 6 lines containing 6 characters each. They are the puzzle's initial position. Those lines contain each character from the string "<span class="tex-font-style-tt">0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ</span>" exactly once.</p>

## Output

<p>On the first line print number <span class="tex-span"><i>n</i></span>, which is the number of operations. On the next <span class="tex-span"><i>n</i></span> lines print the sequence of operations one per line. An operation is described by a word consisting of two characters. The first character shows the direction where the row or the column will be shifted. The possible directions are "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" (to the left, to the right correspondingly, we shift a row), "<span class="tex-font-style-tt">U</span>", "<span class="tex-font-style-tt">D</span>" (upwards, downwards correspondingly, we shift a column). The second character is the number of the row (or the column), it is an integer from "<span class="tex-font-style-tt">1</span>" to "<span class="tex-font-style-tt">6</span>". The rows are numbered from the top to the bottom, the columns are numbered from the left to the right.</p><p>The number of operations should not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. If there are several solutions, print any of them.</p>





```input1
01W345
729AB6
CD8FGH
IJELMN
OPKRST
UVQXYZ

```




```output1
2
R2
U3

```


