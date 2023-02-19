## Description

<div><p>There is a chessboard of size $n$ by $n$. The square in the $i$-th row from top and $j$-th column from the left is labelled $(i,j)$.</p><p>Currently, Gregor has some pawns in the $n$-th row. There are also enemy pawns in the $1$-st row. On one turn, Gregor moves one of <span class="tex-font-style-bf">his</span> pawns. A pawn can move one square up (from $(i,j)$ to $(i-1,j)$) if there is no pawn in the destination square. Additionally, a pawn can move one square diagonally up (from $(i,j)$ to either $(i-1,j-1)$ or $(i-1,j+1)$) if and only if there is an enemy pawn in that square. The enemy pawn is also removed.</p><p>Gregor wants to know what is the maximum number of his pawns that can reach row $1$?</p><p>Note that only Gregor takes turns in this game, and <span class="tex-font-style-bf">the enemy pawns never move</span>. Also, when Gregor's pawn reaches row $1$, it is stuck and cannot make any further moves.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1\le t\le 2\cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of three lines. The first line contains a single integer $n$ ($2\le n\le 2\cdot{10}^{5}$) — the size of the chessboard.</p><p>The second line consists of a string of binary digits of length $n$, where a $1$ in the $i$-th position corresponds to an enemy pawn in the $i$-th cell from the left, and $0$ corresponds to an empty cell.</p><p>The third line consists of a string of binary digits of length $n$, where a $1$ in the $i$-th position corresponds to a Gregor's pawn in the $i$-th cell from the left, and $0$ corresponds to an empty cell.</p><p>It is guaranteed that the sum of $n$ across all test cases is less than $2\cdot{10}^{5}$.</p></div><div class="output-specification"><p>For each test case, print one integer: the <span class="tex-font-style-bf">maximum</span> number of Gregor's pawns which can reach the $1$-st row.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1\le t\le 2\cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of three lines. The first line contains a single integer $n$ ($2\le n\le 2\cdot{10}^{5}$) — the size of the chessboard.</p><p>The second line consists of a string of binary digits of length $n$, where a $1$ in the $i$-th position corresponds to an enemy pawn in the $i$-th cell from the left, and $0$ corresponds to an empty cell.</p><p>The third line consists of a string of binary digits of length $n$, where a $1$ in the $i$-th position corresponds to a Gregor's pawn in the $i$-th cell from the left, and $0$ corresponds to an empty cell.</p><p>It is guaranteed that the sum of $n$ across all test cases is less than $2\cdot{10}^{5}$.</p>

## Output

<p>For each test case, print one integer: the <span class="tex-font-style-bf">maximum</span> number of Gregor's pawns which can reach the $1$-st row.</p>





```input1
4
3
000
111
4
1111
1111
3
010
010
5
11001
00000
```




```output1
3
4
0
0
```



## Note

<p>In the first example, Gregor can simply advance all $3$ of his pawns forward. Thus, the answer is $3$.</p><p>In the second example, Gregor can guarantee that all $4$ of his pawns reach the enemy row, by following the colored paths as demonstrated in the diagram below. Remember, only Gregor takes turns in this "game"!</p><center> <img class="tex-graphics" src="file://VmJ69yM8.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center><p>In the third example, Gregor's only pawn is stuck behind the enemy pawn, and cannot reach the end.</p><p>In the fourth example, Gregor has no pawns, so the answer is clearly $0$.</p>
