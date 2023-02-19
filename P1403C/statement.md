## Description

<div><p>The mythic world of Chess Land is a rectangular grid of squares with $R$ rows and $C$ columns, $R$ being greater than or equal to $C$. Its rows and columns are numbered from $1$ to $R$ and $1$ to $C$, respectively. </p><p>The inhabitants of Chess Land are usually mentioned as <span class="tex-font-style-underline">pieces</span> in everyday language, and there are $5$ specific types of them roaming the land: pawns, rooks, bishops, queens and kings. Contrary to popular belief, chivalry is long dead in Chess Land, so there are no knights to be found.</p><p>Each piece is unique in the way it moves around from square to square: in one step, </p><ul> <li> a pawn can move one row forward (i.e. from row $r$ to $r+1$), without changing columns; </li><li> a rook can move any number of columns left/right without changing rows OR move any number of rows forward/backward without changing columns; </li><li> a bishop can move to any square of the two diagonals intersecting at its currently occupied square; </li><li> a queen can move to any square where a rook or a bishop could move to from her position; </li><li> and a king can move to any of the $8$ adjacent squares. </li></ul> In the following figure, we marked by X the squares each piece can move to in a single step (here, the rows are numbered from bottom to top, and the columns from left to right).<center> <img class="tex-graphics" height="227px" src="file://FCA3piT3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Recently, Chess Land has become a dangerous place: pieces that are passing through the land can get captured unexpectedly by unknown forces and simply disappear. As a consequence, they would like to reach their destinations as fast (i.e. in as few moves) as possible, and they are also interested in the number of different ways it is possible for them to reach it, using the minimal number of steps – because more paths being available could mean lower chances of getting captured. Two paths are considered different if they differ in at least one visited square.</p><p>For this problem, let us assume that pieces are entering Chess Land in a given column of row $1$, and exit the land in a given column of row $R$. Your task is to answer $Q$ questions: given the type of a piece, the column it enters row $1$ and the column it must reach in row $R$ in order to exit, compute the minimal number of moves it has to make in Chess Land, and the number of different ways it is able to do so.</p></div><div class="input-specification"><p>The first line contains three space-separated integers $R$, $C$, and $Q$ $(1 \leq Q \leq 1000$, $2 \leq C \leq 1000$ and $C \leq R \leq 10^9)$ – the number of rows and columns of Chess Land, and the number of questions, respectively. Then $Q$ lines follow.</p><p>Each line consists of </p><ul> <li> a character $T$, corresponding to the type of the piece in question ('P' for pawn, 'R' for rook, 'B' for bishop, 'Q' for queen and 'K' for king); </li><li> two integers $c_1$ and $c_R$, $1\leq c_1,c_R\leq C$, denoting that the piece starts from the $c_1$-th column of row $1$, and has to reach the $c_R$-th column of row $R$. </li></ul></div><div class="output-specification"><p>You have to print $Q$ lines, the $i$-th one containing two space separated integers, the answer to the $i$-th question: the first one is the minimal number of steps needed, the second is the number of different paths available using this number of steps. Since the answer can be quite large, you have to compute it modulo $10^9+7$.</p><p>If it is impossible to reach the target square, output the line "0 0".</p></div><div><h2>Scoring</h2><center> $ \begin{array}{|c|c|l|} \hline \text{Subtask} &amp; \text{Points} &amp; \text{Constraints} \\ \hline 1 &amp; 0 &amp; \text{samples}\\ \hline 2 &amp; 8 &amp; T\in\{\text{'P','R','Q'}\}\text{, i.e. all pieces are pawns, rooks or queens} \\ \hline 3 &amp; 15 &amp; T=\text{'B' and } \: C,R\leq 100 \\ \hline 4 &amp; 22 &amp; T=\text{'B'} \\ \hline 5 &amp; 5 &amp; T=\text{'K' and }\:C,R\leq 100\:\text{and}\:Q\leq 50 \\ \hline 6 &amp; 8 &amp; T=\text{'K' and }\:C,R\leq 100\\ \hline 7 &amp; 15 &amp; T=\text{'K' and }\:C\leq 100\\ \hline 8 &amp; 20 &amp; T=\text{'K'}\\ \hline 9 &amp; 7 &amp; \text{no additional constraints}\\ \hline \end{array} $ </center></div>

## Input

<p>The first line contains three space-separated integers $R$, $C$, and $Q$ $(1 \leq Q \leq 1000$, $2 \leq C \leq 1000$ and $C \leq R \leq 10^9)$ – the number of rows and columns of Chess Land, and the number of questions, respectively. Then $Q$ lines follow.</p><p>Each line consists of </p><ul> <li> a character $T$, corresponding to the type of the piece in question ('P' for pawn, 'R' for rook, 'B' for bishop, 'Q' for queen and 'K' for king); </li><li> two integers $c_1$ and $c_R$, $1\leq c_1,c_R\leq C$, denoting that the piece starts from the $c_1$-th column of row $1$, and has to reach the $c_R$-th column of row $R$. </li></ul>

## Output

<p>You have to print $Q$ lines, the $i$-th one containing two space separated integers, the answer to the $i$-th question: the first one is the minimal number of steps needed, the second is the number of different paths available using this number of steps. Since the answer can be quite large, you have to compute it modulo $10^9+7$.</p><p>If it is impossible to reach the target square, output the line "0 0".</p>





```input1
8 8 5
P 1 2
R 4 8
Q 2 3
B 3 6
K 5 5
```




```output1
0 0
2 2
2 5
2 2
7 393
```



## Note

<p>You can download the above example and an additional (bigger) sample input here: <a href="https://gofile.io/d/GDzwfC">https://gofile.io/d/GDzwfC</a></p>
