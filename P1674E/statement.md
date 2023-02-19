## Description

<div><p>Monocarp plays "Rage of Empires II: Definitive Edition" — a strategic computer game. Right now he's planning to attack his opponent in the game, but Monocarp's forces cannot enter the opponent's territory since the opponent has built a wall.</p><p>The wall consists of $n$ sections, aligned in a row. The $i$-th section initially has durability $a_i$. If durability of some section becomes $0$ or less, this section is considered broken.</p><p>To attack the opponent, Monocarp needs to break at least two sections of the wall (any two sections: possibly adjacent, possibly not). To do this, he plans to use an onager — a special siege weapon. The onager can be used to shoot any section of the wall; the shot deals $2$ damage to the target section and $1$ damage to adjacent sections. In other words, if the onager shoots at the section $x$, then the durability of the section $x$ decreases by $2$, and the durability of the sections $x - 1$ and $x + 1$ (if they exist) decreases by $1$ each. </p><p>Monocarp can shoot at any sections any number of times, <span class="tex-font-style-bf">he can even shoot at broken sections</span>.</p><p>Monocarp wants to calculate the minimum number of onager shots needed to break at least two sections. Help him!</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of sections.</p><p>The second line contains the sequence of integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$), where $a_i$ is the initial durability of the $i$-th section.</p></div><div class="output-specification"><p>Print one integer — the minimum number of onager shots needed to break at least two sections of the wall.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of sections.</p><p>The second line contains the sequence of integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$), where $a_i$ is the initial durability of the $i$-th section.</p>

## Output

<p>Print one integer — the minimum number of onager shots needed to break at least two sections of the wall.</p>





```input1
5
20 10 30 10 20
```




```input2
3
1 8 1
```




```input3
6
7 6 6 8 5 8
```




```input4
6
14 3 8 10 15 4
```




```input5
4
1 100 100 1
```




```input6
3
40 10 10
```




```output1
10
```




```output2
1
```




```output3
4
```




```output4
4
```




```output5
2
```




```output6
7
```



## Note

<p>In the first example, it is possible to break the $2$-nd and the $4$-th section in $10$ shots, for example, by shooting the third section $10$ times. After that, the durabilities become $[20, 0, 10, 0, 20]$. Another way of doing it is firing $5$ shots at the $2$-nd section, and another $5$ shots at the $4$-th section. After that, the durabilities become $[15, 0, 20, 0, 15]$.</p><p>In the second example, it is enough to shoot the $2$-nd section once. Then the $1$-st and the $3$-rd section will be broken.</p><p>In the third example, it is enough to shoot the $2$-nd section twice (then the durabilities become $[5, 2, 4, 8, 5, 8]$), and then shoot the $3$-rd section twice (then the durabilities become $[5, 0, 0, 6, 5, 8]$). So, four shots are enough to break the $2$-nd and the $3$-rd section.</p>
