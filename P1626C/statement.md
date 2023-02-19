## Description

<div><p>Monocarp is playing a computer game once again. He is a wizard apprentice, who only knows a single spell. Luckily, this spell can damage the monsters.</p><p>The level he's currently on contains $n$ monsters. The $i$-th of them appears $k_i$ seconds after the start of the level and has $h_i$ health points. As an additional constraint, $h_i \le k_i$ for all $1 \le i \le n$. All $k_i$ are different.</p><p>Monocarp can cast the spell at moments which are positive integer amounts of second after the start of the level: $1, 2, 3, \dots$ The damage of the spell is calculated as follows. If he didn't cast the spell at the previous second, the damage is $1$. Otherwise, let the damage at the previous second be $x$. Then he can choose the damage to be either $x + 1$ or $1$. A spell uses mana: casting a spell with damage $x$ uses $x$ mana. Mana doesn't regenerate.</p><p>To kill the $i$-th monster, Monocarp has to cast a spell with damage at least $h_i$ at the exact moment the monster appears, which is $k_i$.</p><p>Note that Monocarp can cast the spell even when there is no monster at the current second.</p><p>The mana amount required to cast the spells is the sum of mana usages for all cast spells. Calculate the least amount of mana required for Monocarp to kill all monsters.</p><p>It can be shown that it's always possible to kill all monsters under the constraints of the problem.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of the testcase contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of monsters in the level.</p><p>The second line of the testcase contains $n$ integers $k_1 &lt; k_2 &lt; \dots &lt; k_n$ ($1 \le k_i \le 10^9$)&nbsp;— the number of second from the start the $i$-th monster appears at. All $k_i$ are different, $k_i$ are provided in the increasing order.</p><p>The third line of the testcase contains $n$ integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le k_i \le 10^9$)&nbsp;— the health of the $i$-th monster.</p><p>The sum of $n$ over all testcases doesn't exceed $10^4$.</p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— the least amount of mana required for Monocarp to kill all monsters.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of the testcase contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of monsters in the level.</p><p>The second line of the testcase contains $n$ integers $k_1 &lt; k_2 &lt; \dots &lt; k_n$ ($1 \le k_i \le 10^9$)&nbsp;— the number of second from the start the $i$-th monster appears at. All $k_i$ are different, $k_i$ are provided in the increasing order.</p><p>The third line of the testcase contains $n$ integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le k_i \le 10^9$)&nbsp;— the health of the $i$-th monster.</p><p>The sum of $n$ over all testcases doesn't exceed $10^4$.</p>

## Output

<p>For each testcase, print a single integer&nbsp;— the least amount of mana required for Monocarp to kill all monsters.</p>





```input1
3
1
6
4
2
4 5
2 2
3
5 7 9
2 1 2
```




```output1
10
6
7
```



## Note

<p>In the first testcase of the example, Monocarp can cast spells $3, 4, 5$ and $6$ seconds from the start with damages $1, 2, 3$ and $4$, respectively. The damage dealt at $6$ seconds is $4$, which is indeed greater than or equal to the health of the monster that appears.</p><p>In the second testcase of the example, Monocarp can cast spells $3, 4$ and $5$ seconds from the start with damages $1, 2$ and $3$, respectively.</p><p>In the third testcase of the example, Monocarp can cast spells $4, 5, 7, 8$ and $9$ seconds from the start with damages $1, 2, 1, 1$ and $2$, respectively.</p>
