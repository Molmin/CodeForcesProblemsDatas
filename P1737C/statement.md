## Description

<div><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-left"><img class="tex-graphics" src="file://0GkkXrM8.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-left"><span class="tex-font-style-it">Ela likes Chess a lot. During breaks, she usually challenges her co-worker in DTL to some chess games. She's not an expert at classic chess, but she's very interested in Chess variants, where she has to adapt to new rules and test her tactical mindset to win the game.</span></td></tr></tbody></table><p></p><p>The problem, which involves a non-standard chess pieces type that is described below, reads: given $3$ white <span class="tex-font-style-bf">crickets</span> on a $n \cdot n$ board, arranged in an "L" shape next to each other, there are no other pieces on the board. Ela wants to know with a finite number of moves, can she put any white cricket on the square on row $x$, column $y$?</p><p>An "L"-shape piece arrangement can only be one of the below:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://AKR0oVtA.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://ZFmogzJr.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> </center><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://bTFiAqtj.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://0HF8ZM8Y.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> </center><p>For simplicity, we describe the rules for crickets on the board where only three white crickets are. It can move horizontally, vertically, or diagonally, but only to a square in some direction that is <span class="tex-font-style-bf">immediately after</span> another cricket piece (so that it must <span class="tex-font-style-bf">jump over</span> it). If the square immediately behind the piece is unoccupied, the cricket will occupy the square. Otherwise (when the square is occupied by another cricket, or does not exist), the cricket isn't allowed to make such a move.</p><p>See an example of valid crickets' moves on the pictures in the Note section.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains $n$ ($4 \le n \le 10^5$) — denotes the size of the chessboard.</p><p>The second line of each test case contains 6 numbers: $r_1$, $c_1$, $r_2$, $c_2$, $r_3$, $c_3$ ($1 \le r_1, c_1, r_2, c_2, r_3, c_3 \le n$) — coordinates of the crickets. The input ensures that the three crickets are arranged in an "L" shape that the legend stated.</p><p>The third line of each test case contains 2 numbers: $x$, $y$ ($1 \le x, y \le n$) — coordinates of the target square.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">"YES"</span> or <span class="tex-font-style-tt">"NO"</span> to denotes whether Ela can put a cricket on the target square.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains $n$ ($4 \le n \le 10^5$) — denotes the size of the chessboard.</p><p>The second line of each test case contains 6 numbers: $r_1$, $c_1$, $r_2$, $c_2$, $r_3$, $c_3$ ($1 \le r_1, c_1, r_2, c_2, r_3, c_3 \le n$) — coordinates of the crickets. The input ensures that the three crickets are arranged in an "L" shape that the legend stated.</p><p>The third line of each test case contains 2 numbers: $x$, $y$ ($1 \le x, y \le n$) — coordinates of the target square.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">"YES"</span> or <span class="tex-font-style-tt">"NO"</span> to denotes whether Ela can put a cricket on the target square.</p>





```input1|2,3,4,8,9,10,14,15,16
6
8
7 2 8 2 7 1
5 1
8
2 2 1 2 2 1
5 5
8
2 2 1 2 2 1
6 6
8
1 1 1 2 2 1
5 5
8
2 2 1 2 2 1
8 8
8
8 8 8 7 7 8
4 8
```




```output1
YES
NO
YES
NO
YES
YES
```



## Note

<p>Here's the solution for the first test case. The red square denotes where the crickets need to reach. Note that in chess horizontals are counted from bottom to top, as well as on this picture.</p><center> <img class="tex-graphics" src="file://FnEVDBg5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
