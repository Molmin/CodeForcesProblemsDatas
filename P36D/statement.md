## Description

<div><p>Petya and Vasya are inventing a new game that requires a rectangular board and one chess piece. At the beginning of the game the piece stands in the upper-left corner of the board. Two players move the piece in turns. Each turn the chess piece can be moved either one square to the right or one square down or jump <span class="tex-span"><i>k</i></span> squares diagonally down and to the right. The player who can’t move the piece loses. </p><center> <img class="tex-graphics" src="file://LyQlmj48.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The guys haven’t yet thought what to call the game or the best size of the board for it. Your task is to write a program that can determine the outcome of the game depending on the board size.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 20</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). Each of the following <span class="tex-span"><i>t</i></span> lines contains two numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> — the board’s length and width (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>t</i></span> lines that can determine the outcomes of the game on every board. Write «+» if the first player is a winner, and «-» otherwise.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 20</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). Each of the following <span class="tex-span"><i>t</i></span> lines contains two numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> — the board’s length and width (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output <span class="tex-span"><i>t</i></span> lines that can determine the outcomes of the game on every board. Write «+» if the first player is a winner, and «-» otherwise.</p>





```input1
10 2
1 1
1 2
2 1
2 2
1 3
2 3
3 1
3 2
3 3
4 3

```




```output1
-
+
+
-
-
+
-
+
+
+

```


