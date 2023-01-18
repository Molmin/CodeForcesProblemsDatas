## Description

<div><p>Polycarp plays "Game 23". Initially he has a number $n$ and his goal is to transform it to $m$. In one move, he can multiply $n$ by $2$ or multiply $n$ by $3$. He can perform any number of moves.</p><p>Print the number of moves needed to transform $n$ to $m$. Print <span class="tex-font-style-tt">-1</span> if it is impossible to do so.</p><p>It is easy to prove that any way to transform $n$ to $m$ contains the same number of moves (i.e. number of moves doesn't depend on the way of transformation).</p></div><div class="input-specification"><p>The only line of the input contains two integers $n$ and $m$ ($1 \le n \le m \le 5\cdot10^8$).</p></div><div class="output-specification"><p>Print the number of moves to transform $n$ to $m$, or <span class="tex-font-style-tt">-1</span> if there is no solution.</p></div>

## Input

<p>The only line of the input contains two integers $n$ and $m$ ($1 \le n \le m \le 5\cdot10^8$).</p>

## Output

<p>Print the number of moves to transform $n$ to $m$, or <span class="tex-font-style-tt">-1</span> if there is no solution.</p>





```input1
120 51840
```




```input2
42 42
```




```input3
48 72
```




```output1
7
```




```output2
0
```




```output3
-1
```



## Note

<p>In the first example, the possible sequence of moves is: $120 \rightarrow 240 \rightarrow 720 \rightarrow 1440 \rightarrow 4320 \rightarrow 12960 \rightarrow 25920 \rightarrow 51840.$ The are $7$ steps in total.</p><p>In the second example, no moves are needed. Thus, the answer is $0$.</p><p>In the third example, it is impossible to transform $48$ to $72$.</p>
