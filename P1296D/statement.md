## Description

<div><p>There are $n$ monsters standing in a row numbered from $1$ to $n$. The $i$-th monster has $h_i$ health points (hp). You have your attack power equal to $a$ hp and your opponent has his attack power equal to $b$ hp.</p><p>You and your opponent are fighting these monsters. Firstly, you and your opponent go to the first monster and fight it till his death, then you and your opponent go the second monster and fight it till his death, and so on. A monster is considered dead if its hp is less than or equal to $0$.</p><p>The fight with a monster happens in turns. </p><ol> <li> You hit the monster by $a$ hp. If it is dead after your hit, <span class="tex-font-style-bf">you gain one point</span> and you both proceed to the next monster. </li><li> Your opponent hits the monster by $b$ hp. If it is dead after his hit, <span class="tex-font-style-bf">nobody gains a point</span> and you both proceed to the next monster. </li></ol><p>You have some secret technique to force your opponent to skip his turn. You can use this technique at most $k$ times <span class="tex-font-style-bf">in total</span> (for example, if there are two monsters and $k=4$, then you can use the technique $2$ times on the first monster and $1$ time on the second monster, but not $2$ times on the first monster and $3$ times on the second monster).</p><p>Your task is to determine the maximum number of points you can gain if you use the secret technique optimally.</p></div><div class="input-specification"><p>The first line of the input contains four integers $n, a, b$ and $k$ ($1 \le n \le 2 \cdot 10^5, 1 \le a, b, k \le 10^9$) — the number of monsters, your attack power, the opponent's attack power and the number of times you can use the secret technique.</p><p>The second line of the input contains $n$ integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le 10^9$), where $h_i$ is the health points of the $i$-th monster.</p></div><div class="output-specification"><p>Print one integer — the maximum number of points you can gain if you use the secret technique optimally.</p></div>

## Input

<p>The first line of the input contains four integers $n, a, b$ and $k$ ($1 \le n \le 2 \cdot 10^5, 1 \le a, b, k \le 10^9$) — the number of monsters, your attack power, the opponent's attack power and the number of times you can use the secret technique.</p><p>The second line of the input contains $n$ integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le 10^9$), where $h_i$ is the health points of the $i$-th monster.</p>

## Output

<p>Print one integer — the maximum number of points you can gain if you use the secret technique optimally.</p>





```input1
6 2 3 3
7 10 50 12 1 8
```




```input2
1 1 100 99
100
```




```input3
7 4 2 1
1 3 5 4 2 7 6
```




```output1
5
```




```output2
1
```




```output3
6
```


