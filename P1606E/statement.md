## Description

<div><p>There are $n$ heroes fighting in the arena. Initially, the $i$-th hero has $a_i$ health points.</p><p>The fight in the arena takes place in several rounds. At the beginning of each round, each alive hero deals $1$ damage to all other heroes. Hits of all heroes occur simultaneously. Heroes whose health is less than $1$ at the end of the round are considered killed.</p><p>If exactly $1$ hero remains alive after a certain round, then he is declared the winner. Otherwise, there is no winner.</p><p>Your task is to calculate the number of ways to choose the initial health points for each hero $a_i$, where $1 \le a_i \le x$, so that there is no winner of the fight. The number of ways can be very large, so print it modulo $998244353$. Two ways are considered different if at least one hero has a different amount of health. For example, $[1, 2, 1]$ and $[2, 1, 1]$ are different.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $x$ ($2 \le n \le 500; 1 \le x \le 500$).</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of ways to choose the initial health points for each hero $a_i$, where $1 \le a_i \le x$, so that there is no winner of the fight, taken modulo $998244353$. </p></div>

## Input

<p>The only line contains two integers $n$ and $x$ ($2 \le n \le 500; 1 \le x \le 500$).</p>

## Output

<p>Print one integer&nbsp;— the number of ways to choose the initial health points for each hero $a_i$, where $1 \le a_i \le x$, so that there is no winner of the fight, taken modulo $998244353$. </p>





```input1
2 5
```




```input2
3 3
```




```input3
5 4
```




```input4
13 37
```




```output1
5
```




```output2
15
```




```output3
1024
```




```output4
976890680
```


