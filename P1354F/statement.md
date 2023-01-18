## Description

<div><p>Polycarp plays a computer game. In this game, the players summon armies of magical minions, which then fight each other.</p><p>Polycarp can summon $n$ different minions. The initial power level of the $i$-th minion is $a_i$, and when it is summoned, all previously summoned minions' power levels are increased by $b_i$. The minions can be summoned in any order.</p><p>Unfortunately, Polycarp cannot have more than $k$ minions under his control. To get rid of unwanted minions after summoning them, he may destroy them. Each minion can be summoned (and destroyed) only once.</p><p>Polycarp's goal is to summon the strongest possible army. Formally, he wants to maximize the sum of power levels of all minions under his control (those which are summoned and not destroyed).</p><p>Help Polycarp to make up a plan of actions to summon the strongest possible army!</p></div><div class="input-specification"><p>The first line contains one integer $T$ ($1 \le T \le 75$) — the number of test cases.</p><p>Each test case begins with a line containing two integers $n$ and $k$ ($1 \le k \le n \le 75$) — the number of minions availible for summoning, and the maximum number of minions that can be controlled by Polycarp, respectively.</p><p>Then $n$ lines follow, the $i$-th line contains $2$ integers $a_i$ and $b_i$ ($1 \le a_i \le 10^5$, $0 \le b_i \le 10^5$) — the parameters of the $i$-th minion.</p></div><div class="output-specification"><p>For each test case print the optimal sequence of actions as follows:</p><p>Firstly, print $m$ — the number of actions which Polycarp has to perform ($0 \le m \le 2n$). Then print $m$ integers $o_1$, $o_2$, ..., $o_m$, where $o_i$ denotes the $i$-th action as follows: if the $i$-th action is to summon the minion $x$, then $o_i = x$, and if the $i$-th action is to destroy the minion $x$, then $o_i = -x$. Each minion can be summoned at most once and cannot be destroyed before being summoned (and, obviously, cannot be destroyed more than once). The number of minions in Polycarp's army should be not greater than $k$ after every action.</p><p>If there are multiple optimal sequences, print any of them.</p></div>

## Input

<p>The first line contains one integer $T$ ($1 \le T \le 75$) — the number of test cases.</p><p>Each test case begins with a line containing two integers $n$ and $k$ ($1 \le k \le n \le 75$) — the number of minions availible for summoning, and the maximum number of minions that can be controlled by Polycarp, respectively.</p><p>Then $n$ lines follow, the $i$-th line contains $2$ integers $a_i$ and $b_i$ ($1 \le a_i \le 10^5$, $0 \le b_i \le 10^5$) — the parameters of the $i$-th minion.</p>

## Output

<p>For each test case print the optimal sequence of actions as follows:</p><p>Firstly, print $m$ — the number of actions which Polycarp has to perform ($0 \le m \le 2n$). Then print $m$ integers $o_1$, $o_2$, ..., $o_m$, where $o_i$ denotes the $i$-th action as follows: if the $i$-th action is to summon the minion $x$, then $o_i = x$, and if the $i$-th action is to destroy the minion $x$, then $o_i = -x$. Each minion can be summoned at most once and cannot be destroyed before being summoned (and, obviously, cannot be destroyed more than once). The number of minions in Polycarp's army should be not greater than $k$ after every action.</p><p>If there are multiple optimal sequences, print any of them.</p>





```input1
3
5 2
5 3
7 0
5 0
4 0
10 0
2 1
10 100
50 10
5 5
1 5
2 4
3 3
4 2
5 1
```




```output1
4
2 1 -1 5
1
2
5
5 4 3 2 1
```



## Note

<p>Consider the example test.</p><p>In the first test case, Polycarp can summon the minion $2$ with power level $7$, then summon the minion $1$, which will increase the power level of the previous minion by $3$, then destroy the minion $1$, and finally, summon the minion $5$. After this, Polycarp will have two minions with power levels of $10$.</p><p>In the second test case, Polycarp can control only one minion, so he should choose the strongest of them and summon it.</p><p>In the third test case, Polycarp is able to summon and control all five minions.</p>
