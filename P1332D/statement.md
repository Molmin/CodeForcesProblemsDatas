## Description

<div><p>Bob is playing a game named "Walk on Matrix".</p><p>In this game, player is given an $n \times m$ matrix $A=(a_{i,j})$, i.e. the element in the $i$-th row in the $j$-th column is $a_{i,j}$. Initially, player is located at position $(1,1)$ with score $a_{1,1}$. </p><p>To reach the goal, position $(n,m)$, player can move right or down, i.e. move from $(x,y)$ to $(x,y+1)$ or $(x+1,y)$, as long as player is still on the matrix.</p><p>However, each move changes player's score to the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND</a> of the current score and the value at the position he moves to.</p><p>Bob can't wait to find out the maximum score he can get using the tool he recently learnt &nbsp;— dynamic programming. Here is his algorithm for this problem. </p><center> <img class="tex-graphics" src="file://CcINWnmi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>However, he suddenly realize that the algorithm above fails to output the maximum score for some matrix $A$. Thus, for any given non-negative integer $k$, he wants to find out an $n \times m$ matrix $A=(a_{i,j})$ such that </p><ul> <li> $1 \le n,m \le 500$ (as Bob hates large matrix); </li><li> $0 \le a_{i,j} \le 3 \cdot 10^5$ for all $1 \le i\le n,1 \le j\le m$ (as Bob hates large numbers); </li><li> the difference between the maximum score he can get and the output of his algorithm is <span class="tex-font-style-bf">exactly</span> $k$. </li></ul><p>It can be shown that for any given integer $k$ such that $0 \le k \le 10^5$, there exists a matrix satisfying the above constraints.</p><p>Please help him with it!</p></div><div class="input-specification"><p>The only line of the input contains one single integer $k$ ($0 \le k \le 10^5$).</p></div><div class="output-specification"><p>Output two integers $n$, $m$ ($1 \le n,m \le 500$) in the first line, representing the size of the matrix. </p><p>Then output $n$ lines with $m$ integers in each line, $a_{i,j}$ in the $(i+1)$-th row, $j$-th column.</p></div>

## Input

<p>The only line of the input contains one single integer $k$ ($0 \le k \le 10^5$).</p>

## Output

<p>Output two integers $n$, $m$ ($1 \le n,m \le 500$) in the first line, representing the size of the matrix. </p><p>Then output $n$ lines with $m$ integers in each line, $a_{i,j}$ in the $(i+1)$-th row, $j$-th column.</p>





```input1
0
```




```input2
1
```




```output1
1 1
300000
```




```output2
3 4
7 3 3 1
4 8 3 6
7 7 7 3
```



## Note

<p>In the first example, the maximum score Bob can achieve is $300000$, while the output of his algorithm is $300000$.</p><p>In the second example, the maximum score Bob can achieve is $7\&amp;3\&amp;3\&amp;3\&amp;7\&amp;3=3$, while the output of his algorithm is $2$.</p>
