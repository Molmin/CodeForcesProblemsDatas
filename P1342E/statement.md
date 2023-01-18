## Description

<div><p>Calculate the number of ways to place $n$ rooks on $n \times n$ chessboard so that both following conditions are met:</p><ul> <li> each empty cell is under attack; </li><li> exactly $k$ pairs of rooks attack each other. </li></ul><p>An empty cell is under attack if there is at least one rook in the same row or at least one rook in the same column. Two rooks attack each other if they share the same row or column, <span class="tex-font-style-it">and there are no other rooks between them</span>. For example, there are only two pairs of rooks that attack each other in the following picture:</p><center> <img class="tex-graphics" src="file://hKGrNW6V.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">One of the ways to place the rooks for $n = 3$ and $k = 2$</span> </center><p>Two ways to place the rooks are considered different if there exists at least one cell which is empty in one of the ways but contains a rook in another way.</p><p>The answer might be large, so print it modulo $998244353$.</p></div><div class="input-specification"><p>The only line of the input contains two integers $n$ and $k$ ($1 \le n \le 200000$; $0 \le k \le \frac{n(n - 1)}{2}$).</p></div><div class="output-specification"><p>Print one integer — the number of ways to place the rooks, taken modulo $998244353$.</p></div>

## Input

<p>The only line of the input contains two integers $n$ and $k$ ($1 \le n \le 200000$; $0 \le k \le \frac{n(n - 1)}{2}$).</p>

## Output

<p>Print one integer — the number of ways to place the rooks, taken modulo $998244353$.</p>





```input1
3 2
```




```input2
3 3
```




```input3
4 0
```




```input4
1337 42
```




```output1
6
```




```output2
0
```




```output3
24
```




```output4
807905441
```


