## Description

<div><p>Marina plays a new rogue-like game. In this game, there are $n$ different character species and $m$ different classes. The game is played in runs; for each run, Marina has to select a species and a class for her character. If she selects the $i$-th species and the $j$-th class, she will get $c_{i, j}$ points for this run.</p><p>Initially, some species and classes are unlocked, all others are locked. To unlock the $i$-th species, Marina has to get at least $a_i$ points in total for previous runs — that is, as soon as her total score for played runs is at least $a_i$, this species is unlocked. Similarly, to unlock the $j$-th class, she has to get at least $b_j$ points in total for previous runs. If $a_i = 0$ for some $i$, then this species is unlocked initially (the same applies to classes with $b_j = 0$).</p><p>Marina wants to unlock all species and classes in the minimum number of runs. Before playing the game, she can read <span class="tex-font-style-bf">exactly one guide</span> on some combination of species and class, and reading a guide will increase the score she gets for <span class="tex-font-style-bf">all runs with that combination</span> by $k$ (formally, before playing the game, she can increase <span class="tex-font-style-bf">exactly one</span> value of $c_{i, j}$ by $k$).</p><p>What is the minimum number of runs she has to play to unlock all species and classes if she chooses the combination to read a guide on optimally?</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $k$ ($1 \le n, m \le 1500$; $0 \le k \le 10^9$).</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($0 = a_1 \le a_2 \le \dots \le a_n \le 10^{12}$), where $a_i$ is the number of points required to unlock the $i$-th species (or $0$, if it is unlocked initially). <span class="tex-font-style-bf">Note that $a_1 = 0$, and these values are non-descending</span>.</p><p>The third line contains $m$ integers $b_1$, $b_2$, ..., $b_m$ ($0 = b_1 \le b_2 \le \dots \le b_m \le 10^{12}$), where $b_i$ is the number of points required to unlock the $i$-th class (or $0$, if it is unlocked initially). <span class="tex-font-style-bf">Note that $b_1 = 0$, and these values are non-descending</span>.</p><p>Then $n$ lines follow, each of them contains $m$ integers. The $j$-th integer in the $i$-th line is $c_{i, j}$ ($1 \le c_{i, j} \le 10^9$) — the score Marina gets for a run with the $i$-th species and the $j$-th class.</p></div><div class="output-specification"><p>Print one integer — the minimum number of runs Marina has to play to unlock all species and all classes if she can read exactly one guide before playing the game.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $k$ ($1 \le n, m \le 1500$; $0 \le k \le 10^9$).</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($0 = a_1 \le a_2 \le \dots \le a_n \le 10^{12}$), where $a_i$ is the number of points required to unlock the $i$-th species (or $0$, if it is unlocked initially). <span class="tex-font-style-bf">Note that $a_1 = 0$, and these values are non-descending</span>.</p><p>The third line contains $m$ integers $b_1$, $b_2$, ..., $b_m$ ($0 = b_1 \le b_2 \le \dots \le b_m \le 10^{12}$), where $b_i$ is the number of points required to unlock the $i$-th class (or $0$, if it is unlocked initially). <span class="tex-font-style-bf">Note that $b_1 = 0$, and these values are non-descending</span>.</p><p>Then $n$ lines follow, each of them contains $m$ integers. The $j$-th integer in the $i$-th line is $c_{i, j}$ ($1 \le c_{i, j} \le 10^9$) — the score Marina gets for a run with the $i$-th species and the $j$-th class.</p>

## Output

<p>Print one integer — the minimum number of runs Marina has to play to unlock all species and all classes if she can read exactly one guide before playing the game.</p>





```input1
3 4 2
0 5 7
0 2 6 10
2 5 5 2
5 3 4 4
3 4 2 4
```




```input2
4 2 1
0 3 9 9
0 2
3 3
5 1
1 3
2 3
```




```input3
3 3 5
0 8 11
0 0 3
3 1 3
1 2 1
1 1 3
```




```output1
3
```




```output2
2
```




```output3
2
```



## Note

<p>The explanation for the first test:</p><ol> <li> Marina reads a guide on the combination of the $1$-st species and the $2$-nd class. Thus, $c_{1, 2}$ becomes $7$. Initially, only the $1$-st species and the $1$-st class are unlocked. </li><li> Marina plays a run with the $1$-st species and the $1$-st class. Her score becomes $2$, and she unlocks the $2$-nd class. </li><li> Marina plays a run with the $1$-st species and the $2$-nd class. Her score becomes $9$, and she unlocks everything except the $4$-th class. </li><li> Marina plays a run with the $3$-rd species and the $3$-rd class. Her score becomes $11$, and she unlocks the $4$-th class. She has unlocked everything in $3$ runs. </li></ol><p>Note that this way to unlock everything is not the only one.</p><p>The explanation for the second test:</p><ol> <li> Marina reads a guide on the combination of the $2$-nd species and the $1$-st class. Thus, $c_{2, 1}$ becomes $6$. Initially, only the $1$-st species and the $1$-st class are unlocked. </li><li> Marina plays a run with the $1$-st species and the $1$-st class. Her score becomes $3$, and she unlocks the $2$-nd species and the $2$-nd class. </li><li> Marina plays a run with the $2$-nd species and the $1$-st class. Her score becomes $9$, and she unlocks the $3$-rd species and the $4$-th species. She has unlocked everything in $2$ runs. </li></ol><p>As in the $1$-st example, this is not the only way to unlock everything in $2$ runs.</p>
