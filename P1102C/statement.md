## Description

<div><p>You are policeman and you are playing a game with Slavik. The game is turn-based and each turn consists of two phases. During the first phase you make your move and during the second phase Slavik makes his move.</p><p>There are $n$ doors, the $i$-th door initially has durability equal to $a_i$.</p><p>During your move you can try to break one of the doors. If you choose door $i$ and its current durability is $b_i$ then you reduce its durability to $max(0, b_i - x)$ (the value $x$ is given).</p><p>During Slavik's move he tries to repair one of the doors. If he chooses door $i$ and its current durability is $b_i$ then he increases its durability to $b_i + y$ (the value $y$ is given). <span class="tex-font-style-bf">Slavik cannot repair doors with current durability equal to $0$</span>.</p><p>The game lasts $10^{100}$ turns. If some player cannot make his move then he has to skip it.</p><p>Your goal is to maximize the number of doors with durability equal to $0$ at the end of the game. You can assume that Slavik <span class="tex-font-style-bf">wants to minimize</span> the number of such doors. What is the number of such doors in the end if you both play optimally?</p></div><div class="input-specification"><p>The first line of the input contains three integers $n$, $x$ and $y$ ($1 \le n \le 100$, $1 \le x, y \le 10^5$) — the number of doors, value $x$ and value $y$, respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$), where $a_i$ is the initial durability of the $i$-th door.</p></div><div class="output-specification"><p>Print one integer — the number of doors with durability equal to $0$ at the end of the game, if you and Slavik both play optimally.</p></div>

## Input

<p>The first line of the input contains three integers $n$, $x$ and $y$ ($1 \le n \le 100$, $1 \le x, y \le 10^5$) — the number of doors, value $x$ and value $y$, respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$), where $a_i$ is the initial durability of the $i$-th door.</p>

## Output

<p>Print one integer — the number of doors with durability equal to $0$ at the end of the game, if you and Slavik both play optimally.</p>





```input1
6 3 2
2 3 1 3 4 2
```




```input2
5 3 3
1 2 4 2 3
```




```input3
5 5 6
1 2 6 10 3
```




```output1
6
```




```output2
2
```




```output3
2
```



## Note

<p>Clarifications about the optimal strategy will be ignored.</p>
