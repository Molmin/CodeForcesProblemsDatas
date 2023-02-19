## Description

<div><p>Genie is taking part in an intellectual game. The game consists of $n$ questions, and there are $m$ participants numbered from $1$ to $m$. Genie is the participant number $1$.</p><p>For each question $i$ and participant $j$, it is known whether the participant will answer the question correctly or not.</p><p>The goal of the game is to be the last participant staying in the game.</p><p>The game is conducted as follows. First, all $n$ questions get shuffled uniformly at random (all $n!$ permutations are equally likely). Then, the questions are asked one by one. Each participant answers the question. If all participants still in the game answer the question correctly, or if all of them answer the question incorrectly, nothing happens. Otherwise, those participants who answer the question incorrectly lose and leave the game.</p><p>After all $n$ questions are asked, all participants who are still in the game are declared to be the winners.</p><p>What is the probability that Genie will win the game?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$&nbsp;— the number of questions and the number of participants ($1 \le n \le 2 \cdot 10^5$; $2 \le m \le 17$).</p><p>The $i$-th of the next $n$ lines contains $m$ characters $s_{i, 1}, s_{i, 2}, \ldots, s_{i, m}$. Character $s_{i, j}$ is '<span class="tex-font-style-tt">1</span>' if participant $j$ answers question $i$ correctly or '<span class="tex-font-style-tt">0</span>' otherwise.</p></div><div class="output-specification"><p>Print the probability that Genie will win the game. Your answer will be considered correct if its absolute or relative error does not exceed $10^{-9}$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$&nbsp;— the number of questions and the number of participants ($1 \le n \le 2 \cdot 10^5$; $2 \le m \le 17$).</p><p>The $i$-th of the next $n$ lines contains $m$ characters $s_{i, 1}, s_{i, 2}, \ldots, s_{i, m}$. Character $s_{i, j}$ is '<span class="tex-font-style-tt">1</span>' if participant $j$ answers question $i$ correctly or '<span class="tex-font-style-tt">0</span>' otherwise.</p>

## Output

<p>Print the probability that Genie will win the game. Your answer will be considered correct if its absolute or relative error does not exceed $10^{-9}$.</p>





```input1
1 5
11010
```




```input2
3 3
011
101
110
```




```input3
6 4
1011
0110
1111
0110
0000
1101
```




```output1
1.0000000000000000
```




```output2
0.3333333333333333
```




```output3
0.1666666666666667
```



## Note

<p>In the first example, there is a single question and Genie will answer it correctly, thus winning the game (along with participants $2$ and $4$).</p><p>In the second example, one participant will leave after the first asked question, and another participant will leave after the second asked question. Each participant will win with probability&nbsp;$\frac{1}{3}$.</p>
