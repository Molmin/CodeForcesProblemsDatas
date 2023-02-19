## Description

<div><p>Alice and Bob play a game. They have a set that initially consists of $n$ integers. The game is played in $k$ turns. During each turn, the following events happen:</p><ol> <li> firstly, Alice chooses an integer from the set. She can choose any integer <span class="tex-font-style-bf">except for the maximum one</span>. Let the integer chosen by Alice be $a$; </li><li> secondly, Bob chooses an integer from the set. He can choose any integer <span class="tex-font-style-bf">that is greater than $a$</span>. Let the integer chosen by Bob be $b$; </li><li> finally, both $a$ and $b$ are erased from the set, and the value of $b - a$ is added to the score of the game. </li></ol><p>Initially, the score is $0$. Alice wants to maximize the resulting score, Bob wants to minimize it. Assuming that both Alice and Bob play optimally, calculate the resulting score of the game.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \le n \le 400$, $1 \le k \le \lfloor\frac{n}{2}\rfloor$) — the initial size of the set and the number of turns in the game.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$) — the initial contents of the set. These integers are pairwise distinct.</p></div><div class="output-specification"><p>Print one integer — the resulting score of the game (assuming that both Alice and Bob play optimally).</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \le n \le 400$, $1 \le k \le \lfloor\frac{n}{2}\rfloor$) — the initial size of the set and the number of turns in the game.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$) — the initial contents of the set. These integers are pairwise distinct.</p>

## Output

<p>Print one integer — the resulting score of the game (assuming that both Alice and Bob play optimally).</p>





```input1
5 2
3 4 1 5 2
```




```input2
7 3
101 108 200 1 201 109 100
```




```output1
4
```




```output2
283
```


