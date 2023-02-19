## Description

<div><p>Pak Chanek, a renowned scholar, invented a card puzzle using his knowledge. In the puzzle, you are given a board with $n$ rows and $m$ columns. Let $(r, c)$ represent the cell in the $r$-th row and the $c$-th column.</p><p>Initially, there are $k$ cards stacked in cell $(1, 1)$. Each card has an integer from $1$ to $k$ written on it. More specifically, the $i$-th card <span class="tex-font-style-bf">from the top</span> of the stack in cell $(1, 1)$ has the number $a_i$ written on it. It is known that no two cards have the same number written on them. In other words, the numbers written on the cards are a permutation of integers from $1$ to $k$. All other cells are empty.</p><p>You need to move the $k$ cards to cell $(n, m)$ to create another stack of cards. Let $b_i$ be the number written on the $i$-th card <span class="tex-font-style-bf">from the top</span> of the stack in cell $(n, m)$. You should create the stack in cell $(n, m)$ in such a way so that $b_i = i$ for all $1 \leq i \leq k$.</p><p>In one move, you can remove the <span class="tex-font-style-bf">top card</span> from a cell and place it onto an adjacent cell (a cell that shares a common side). If the target cell already contains one or more cards, you place your card <span class="tex-font-style-bf">on the top of the stack</span>. You must do each operation while satisfying the following restrictions: </p><ul> <li> Each cell other than $(1,1)$ and $(n,m)$ must not have more than one card on it. </li><li> You cannot move a card onto cell $(1,1)$. </li><li> You cannot move a card from cell $(n,m)$. </li></ul><p>Given the values of $n$, $m$, $k$ and the array $a$, determine if the puzzle is solvable.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 2 \cdot 10^4$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($3 \leq n, m \leq 10^6$, $nm \leq 10^6$, $1 \leq k \leq 10^5$) — the size of the board and the number of cards.</p><p>The second line of the test case contains $k$ integers $a_1, a_2, \ldots, a_k$ — the array $a$, representing the numbers written on the cards. The values of $a$ are a permutation of integers from $1$ to $k$.</p><p>It is guaranteed that the sum of $nm$ and $k$ over all test cases do not exceed $10^6$ and $10^5$ respectively.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YA</span>" (without quotes) if it is possible and "<span class="tex-font-style-tt">TIDAK</span>" (without quotes) otherwise, which mean yes and no in Indonesian respectively.</p><p>You can output "<span class="tex-font-style-tt">YA</span>" and "<span class="tex-font-style-tt">TIDAK</span>" in any case (for example, strings "<span class="tex-font-style-tt">tiDAk</span>", "<span class="tex-font-style-tt">tidak</span>", and "<span class="tex-font-style-tt">Tidak</span>" will be recognised as a negative response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 2 \cdot 10^4$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($3 \leq n, m \leq 10^6$, $nm \leq 10^6$, $1 \leq k \leq 10^5$) — the size of the board and the number of cards.</p><p>The second line of the test case contains $k$ integers $a_1, a_2, \ldots, a_k$ — the array $a$, representing the numbers written on the cards. The values of $a$ are a permutation of integers from $1$ to $k$.</p><p>It is guaranteed that the sum of $nm$ and $k$ over all test cases do not exceed $10^6$ and $10^5$ respectively.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YA</span>" (without quotes) if it is possible and "<span class="tex-font-style-tt">TIDAK</span>" (without quotes) otherwise, which mean yes and no in Indonesian respectively.</p><p>You can output "<span class="tex-font-style-tt">YA</span>" and "<span class="tex-font-style-tt">TIDAK</span>" in any case (for example, strings "<span class="tex-font-style-tt">tiDAk</span>", "<span class="tex-font-style-tt">tidak</span>", and "<span class="tex-font-style-tt">Tidak</span>" will be recognised as a negative response).</p>





```input1|2,3,6,7
4
3 3 6
3 6 4 1 2 5
3 3 10
1 2 3 4 5 6 7 8 9 10
5 4 4
2 1 3 4
3 4 10
10 4 9 3 5 6 8 2 7 1
```




```output1
YA
TIDAK
YA
YA
```



## Note

<p>In the first test case, the following is one way the puzzle can be done: </p><ul> <li> Move the card with $3$ written on it from cell $(1, 1)$ to cell $(1, 2)$, then cell $(1, 3)$. </li><li> Move the card with $6$ written on it from cell $(1, 1)$ to cell $(2, 1)$, then cell $(3, 1)$, then cell $(3, 2)$, then cell $(3, 3)$. </li><li> Move the card with $4$ written on it from cell $(1, 1)$ to cell $(1, 2)$. </li><li> Move the card with $1$ written on it from cell $(1, 1)$ to cell $(2, 1)$, then cell $(2, 2)$, then cell $(2, 3)$. </li><li> Move the card with $2$ written on it from cell $(1, 1)$ to cell $(2, 1)$, then cell $(2, 2)$. </li><li> Move the card with $5$ written on it from cell $(1, 1)$ to cell $(2, 1)$, then cell $(3, 1)$, then cell $(3, 2)$, then cell $(3, 3)$. </li><li> Move the card with $2$ written on it from cell $(2, 2)$ to cell $(2, 1)$. </li><li> Move the card with $4$ written on it from cell $(1, 2)$ to cell $(2, 2)$, then cell $(3, 2)$, then cell $(3, 3)$. </li><li> Move the card with $3$ written on it from cell $(1, 3)$ to cell $(1, 2)$, then cell $(2, 2)$, then cell $(3, 2)$, then cell $(3, 3)$. </li><li> Move the card with $2$ written on it from cell $(2, 1)$ to cell $(3, 1)$, then cell $(3, 2)$, then cell $(3, 3)$. </li><li> Move the card with $1$ written on it from cell $(2, 3)$ to cell $(3, 3)$. </li></ul><p>An animated illustration regarding the process mentioned above is as follows: <img class="tex-graphics" src="file://xK8jluMn.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
