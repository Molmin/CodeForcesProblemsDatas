## Description

<div><p>Chouti was doing a competitive programming competition. However, after having all the problems accepted, he got bored and decided to invent some small games.</p><p>He came up with the following game. The player has a positive integer $n$. Initially the value of $n$ equals to $v$ and the player is able to do the following operation as many times as the player want (possibly zero): choose a positive integer $x$ that $x&lt;n$ and $x$ is not a divisor of $n$, then subtract $x$ from $n$. The goal of the player is to minimize the value of $n$ in the end.</p><p>Soon, Chouti found the game trivial. Can you also beat the game?</p></div><div class="input-specification"><p>The input contains only one integer in the first line: $v$ ($1 \le v \le 10^9$), the initial value of $n$.</p></div><div class="output-specification"><p>Output a single integer, the minimum value of $n$ the player can get.</p></div>

## Input

<p>The input contains only one integer in the first line: $v$ ($1 \le v \le 10^9$), the initial value of $n$.</p>

## Output

<p>Output a single integer, the minimum value of $n$ the player can get.</p>





```input1
8
```




```input2
1
```




```output1
1
```




```output2
1
```



## Note

<p>In the first example, the player can choose $x=3$ in the first turn, then $n$ becomes $5$. He can then choose $x=4$ in the second turn to get $n=1$ as the result. There are other ways to get this minimum. However, for example, he cannot choose $x=2$ in the first turn because $2$ is a divisor of $8$.</p><p>In the second example, since $n=1$ initially, the player can do nothing.</p>
