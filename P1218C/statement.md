## Description

<div><p>You, the mighty Blackout, are standing in the upper-left $(0,0)$ corner of $N$x$M$ matrix. You must move either right or down each second. </p><p>There are $K$ transformers jumping around the matrix in the following way. Each transformer starts jumping from position $(x,y)$, at time $t$, and jumps to the next position each second. The $x$-axes grows downwards, and $y$-axes grows to the right. The order of jumping positions is defined as ${(x,y),(x+d,y-d),(x+d,y),(x,y+d)}$, and is periodic. Before time $t$ transformer is not in the matrix.</p><p>You want to arrive to the bottom-right corner $(N-1,M-1)$, while slaying transformers and losing the least possible amount of energy. When you meet the transformer (or more of them) in the matrix field, you must kill them all, and you lose the sum of the energy amounts required to kill each transformer.</p><p>After the transformer is killed, he of course stops jumping, falls into the abyss and leaves the matrix world. Output minimum possible amount of energy wasted.</p></div><div class="input-specification"><p>In the first line, integers $N$,$M$ ($1 \leq N, M \leq 500$), representing size of the matrix, and $K$ ($0 \leq K \leq 5*10^5$) , the number of jumping transformers.</p><p>In next $K$ lines, for each transformer, numbers $x$, $y$, $d$ ($d \geq 1$), $t$ ($0 \leq t \leq N+M-2$), and $e$ ($0 \leq e \leq 10^9$), representing starting coordinates of transformer, jumping positions distance in pattern described above, time when transformer starts jumping, and energy required to kill it.</p><p>It is guaranteed that all 4 of jumping points of the transformers are within matrix coordinates</p></div><div class="output-specification"><p>Print single integer, the minimum possible amount of energy wasted, for Blackout to arrive at bottom-right corner.</p></div>

## Input

<p>In the first line, integers $N$,$M$ ($1 \leq N, M \leq 500$), representing size of the matrix, and $K$ ($0 \leq K \leq 5*10^5$) , the number of jumping transformers.</p><p>In next $K$ lines, for each transformer, numbers $x$, $y$, $d$ ($d \geq 1$), $t$ ($0 \leq t \leq N+M-2$), and $e$ ($0 \leq e \leq 10^9$), representing starting coordinates of transformer, jumping positions distance in pattern described above, time when transformer starts jumping, and energy required to kill it.</p><p>It is guaranteed that all 4 of jumping points of the transformers are within matrix coordinates</p>

## Output

<p>Print single integer, the minimum possible amount of energy wasted, for Blackout to arrive at bottom-right corner.</p>





```input1
3 3 5
0 1 1 0 7
1 1 1 0 10
1 1 1 1 2
1 1 1 2 2
0 1 1 2 3
```




```output1
9
```



## Note

<p>If Blackout takes the path from (0, 0) to (2, 0), and then from (2, 0) to (2, 2) he will need to kill the first and third transformer for a total energy cost of 9. There exists no path with less energy value.</p>
