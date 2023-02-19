## Description

<div><p>You are playing a new computer game in which you have to fight monsters. In a dungeon you are trying to clear, you met three monsters; the first of them has $a$ health points, the second has $b$ health points, and the third has $c$.</p><p>To kill the monsters, you can use a cannon that, when fired, deals $1$ damage to the selected monster. Every $7$-th (i.&nbsp;e. shots with numbers $7$, $14$, $21$ etc.) cannon shot is <span class="tex-font-style-it">enhanced</span> and deals $1$ damage to <span class="tex-font-style-bf">all</span> monsters, not just one of them. If some monster's current amount of health points is $0$, it can't be targeted by a regular shot and does not receive damage from an <span class="tex-font-style-it">enhanced</span> shot.</p><p>You want to pass the dungeon beautifully, i.&nbsp;e., kill all the monsters with the same <span class="tex-font-style-it">enhanced</span> shot (i.&nbsp;e. after some <span class="tex-font-style-it">enhanced</span> shot, the health points of each of the monsters should become equal to $0$ <span class="tex-font-style-bf">for the first time</span>). Each shot must hit a monster, i.&nbsp;e. each shot deals damage to at least one monster.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of a single line that contains three integers $a$, $b$ and $c$ ($1 \le a, b, c \le 10^8$) — the number of health points each monster has.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if you can kill all the monsters with the same <span class="tex-font-style-it">enhanced</span> shot. Otherwise, print <span class="tex-font-style-tt">NO</span>. You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of a single line that contains three integers $a$, $b$ and $c$ ($1 \le a, b, c \le 10^8$) — the number of health points each monster has.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if you can kill all the monsters with the same <span class="tex-font-style-it">enhanced</span> shot. Otherwise, print <span class="tex-font-style-tt">NO</span>. You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer).</p>





```input1
3
3 2 4
1 1 1
10 1 7
```




```output1
YES
NO
NO
```



## Note

<p>In the first test case, you can do as follows: $1$-th shot to the first monster, $2$-th shot to the second monster, $3$-th shot to the third monster, $4$-th shot to the first monster, $5$-th shot to the third monster, $6$-th shot to the third monster, and $7$-th <span class="tex-font-style-it">enhanced</span> shot will kill all the monsters.</p><p>In the second test case, you can't kill monsters with the same <span class="tex-font-style-it">enhanced</span> shot, because the total number of health points of monsters is $3$, and you will kill them in the first 3 shots.</p>
