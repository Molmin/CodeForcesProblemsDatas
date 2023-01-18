## Description

<div><p>Polycarp has recently got himself a new job. He now earns so much that his old wallet can't even store all the money he has.</p><p>Berland bills somehow come in lots of different sizes. However, all of them are shaped as rectangles (possibly squares). All wallets are also produced in form of rectangles (possibly squares).</p><p>A bill $x \times y$ fits into some wallet $h \times w$ if either $x \le h$ and $y \le w$ or $y \le h$ and $x \le w$. Bills can overlap with each other in a wallet and an infinite amount of bills can fit into a wallet. That implies that all the bills Polycarp currently have fit into a wallet if every single one of them fits into it independently of the others.</p><p>Now you are asked to perform the queries of two types:</p><ol> <li> $+~x~y$ — Polycarp earns a bill of size $x \times y$; </li><li> $?~h~w$ — Polycarp wants to check if all the bills he has earned to this moment fit into a wallet of size $h \times w$. </li></ol><p>It is guaranteed that there is at least one query of type $1$ before the first query of type $2$ and that there is at least one query of type $2$ in the input data.</p><p>For each query of type $2$ print "<span class="tex-font-style-tt">YES</span>" if all the bills he has earned to this moment fit into a wallet of given size. Print "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 5 \cdot 10^5$) — the number of queries.</p><p>Each of the next $n$ lines contains a query of one of these two types:</p><ol> <li> $+~x~y$ ($1 \le x, y \le 10^9$) — Polycarp earns a bill of size $x \times y$; </li><li> $?~h~w$ ($1 \le h, w \le 10^9$) — Polycarp wants to check if all the bills he has earned to this moment fit into a wallet of size $h \times w$. </li></ol><p>It is guaranteed that there is at least one query of type $1$ before the first query of type $2$ and that there is at least one query of type $2$ in the input data.</p></div><div class="output-specification"><p>For each query of type $2$ print "<span class="tex-font-style-tt">YES</span>" if all the bills he has earned to this moment fit into a wallet of given size. Print "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 5 \cdot 10^5$) — the number of queries.</p><p>Each of the next $n$ lines contains a query of one of these two types:</p><ol> <li> $+~x~y$ ($1 \le x, y \le 10^9$) — Polycarp earns a bill of size $x \times y$; </li><li> $?~h~w$ ($1 \le h, w \le 10^9$) — Polycarp wants to check if all the bills he has earned to this moment fit into a wallet of size $h \times w$. </li></ol><p>It is guaranteed that there is at least one query of type $1$ before the first query of type $2$ and that there is at least one query of type $2$ in the input data.</p>

## Output

<p>For each query of type $2$ print "<span class="tex-font-style-tt">YES</span>" if all the bills he has earned to this moment fit into a wallet of given size. Print "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
9
+ 3 2
+ 2 3
? 1 20
? 3 3
? 2 3
+ 1 5
? 10 10
? 1 5
+ 1 1
```




```output1
NO
YES
YES
YES
NO
```



## Note

<p>The queries of type $2$ of the example:</p><ol> <li> Neither bill fits; </li><li> Both bills fit (just checking that you got that bills can overlap); </li><li> Both bills fit (both bills are actually the same); </li><li> All bills fit (too much of free space in a wallet is not a problem); </li><li> Only bill $1 \times 5$ fit (all the others don't, thus it's "<span class="tex-font-style-tt">NO</span>"). </li></ol>
