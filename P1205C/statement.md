## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem</span></p><p>You are given a grid $n\times n$, where $n$ is <span class="tex-font-style-bf">odd</span>. Rows are enumerated from $1$ to $n$ from up to down, columns are enumerated from $1$ to $n$ from left to right. Cell, standing on the intersection of row $x$ and column $y$, is denoted by $(x, y)$.</p><p>Every cell contains $0$ or $1$. It is known that the top-left cell contains $1$, and the bottom-right cell contains $0$.</p><p>We want to know numbers in all cells of the grid. To do so we can ask the following questions: </p><p>"<span class="tex-font-style-tt">$?$ $x_1$ $y_1$ $x_2$ $y_2$</span>", where $1 \le x_1 \le x_2 \le n$, $1 \le y_1 \le y_2 \le n$, and $x_1 + y_1 + 2 \le x_2 + y_2$. In other words, we output two different cells $(x_1, y_1)$, $(x_2, y_2)$ of the grid such that we can get from the first to the second by moving only to the right and down, and they aren't adjacent.</p><p>As a response to such question you will be told if there exists a path between $(x_1, y_1)$ and $(x_2, y_2)$, going only to the right or down, numbers in cells of which form a palindrome.</p><p>For example, paths, shown in green, are palindromic, so answer for "<span class="tex-font-style-tt">$?$ $1$ $1$ $2$ $3$</span>" and "<span class="tex-font-style-tt">$?$ $1$ $2$ $3$ $3$</span>" would be that there exists such path. However, there is no palindromic path between $(1, 1)$ and $(3, 1)$.</p><center> <img class="tex-graphics" src="file://rKizU3zx.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Determine all cells of the grid by asking not more than $n^2$ questions. It can be shown that the answer always exists.</p></div><div class="input-specification"><p>The first line contains <span class="tex-font-style-bf">odd</span> integer ($3 \le n &lt; 50$)&nbsp;— the side of the grid.</p></div><div><h2>Interaction</h2><p>You begin the interaction by reading $n$.</p><p>To ask a question about cells $(x_1, y_1), (x_2, y_2)$, in a separate line output "<span class="tex-font-style-tt">$?$ $x_1$ $y_1$ $x_2$ $y_2$</span>".</p><p>Numbers in the query have to satisfy $1 \le x_1 \le x_2 \le n$, $1 \le y_1 \le y_2 \le n$, and $x_1 + y_1 + 2 \le x_2 + y_2$. Don't forget to 'flush', to get the answer.</p><p>In response, you will receive $1$, if there exists a path going from $(x_1, y_1)$ to $(x_2, y_2)$ only to the right or down, numbers in cells of which form a palindrome, and $0$ otherwise.</p><p>In case your query is invalid or you asked more than $n^2$ queries, program will print $-1$ and will finish interaction. You will receive <span class="tex-font-style-bf">Wrong answer</span> verdict. Make sure to exit immediately to avoid getting other verdicts.</p><p>When you determine numbers in all cells, output "<span class="tex-font-style-tt">!</span>".</p><p>Then output $n$ lines, the $i$-th of which is a string of length $n$, corresponding to numbers in the $i$-th row of the grid.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hack Format</span></p><p>To hack, use the following format.</p><p>The first line should contain a single odd integer $n$ (side of your grid).</p><p>The $i$-th of $n$ following lines should contain a string of length $n$ corresponding to the $i$-th row of the grid. Top left element of the grid has to be equal to $1$, bottom right has to be equal to $0$.</p></div>

## Input

<p>The first line contains <span class="tex-font-style-bf">odd</span> integer ($3 \le n &lt; 50$)&nbsp;— the side of the grid.</p>





```input1
3
0
1
0
1
1
1
1
```




```output1
? 1 1 1 3
? 1 1 2 3
? 2 1 2 3
? 3 1 3 3
? 2 2 3 3
? 1 2 3 2
? 1 2 3 3
!
100
001
000
```


