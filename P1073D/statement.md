## Description

<div><p>XXI Berland Annual Fair is coming really soon! Traditionally fair consists of $n$ booths, arranged in a circle. The booths are numbered $1$ through $n$ clockwise with $n$ being adjacent to $1$. The $i$-th booths sells some candies for the price of $a_i$ burles per item. Each booth has an unlimited supply of candies.</p><p>Polycarp has decided to spend at most $T$ burles at the fair. However, he has some plan in mind for his path across the booths:</p><ul> <li> at first, he visits booth number $1$; </li><li> if he has enough burles to buy <span class="tex-font-style-bf">exactly one</span> candy from the current booth, then he buys it immediately; </li><li> then he proceeds to the next booth in the clockwise order (regardless of if he bought a candy or not). </li></ul><p>Polycarp's money is finite, thus the process will end once he can no longer buy candy at any booth.</p><p>Calculate the number of candies Polycarp will buy.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $T$ ($1 \le n \le 2 \cdot 10^5$, $1 \le T \le 10^{18}$) — the number of booths at the fair and the initial amount of burles Polycarp has.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) — the price of the single candy at booth number $i$.</p></div><div class="output-specification"><p>Print a single integer — the total number of candies Polycarp will buy.</p></div>

## Input

<p>The first line contains two integers $n$ and $T$ ($1 \le n \le 2 \cdot 10^5$, $1 \le T \le 10^{18}$) — the number of booths at the fair and the initial amount of burles Polycarp has.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) — the price of the single candy at booth number $i$.</p>

## Output

<p>Print a single integer — the total number of candies Polycarp will buy.</p>





```input1
3 38
5 2 5

```




```input2
5 21
2 4 100 2 6

```




```output1
10

```




```output2
6

```



## Note

<p>Let's consider the first example. Here are Polycarp's moves until he runs out of money:</p><ol> <li> Booth $1$, buys candy for $5$, $T = 33$; </li><li> Booth $2$, buys candy for $2$, $T = 31$; </li><li> Booth $3$, buys candy for $5$, $T = 26$; </li><li> Booth $1$, buys candy for $5$, $T = 21$; </li><li> Booth $2$, buys candy for $2$, $T = 19$; </li><li> Booth $3$, buys candy for $5$, $T = 14$; </li><li> Booth $1$, buys candy for $5$, $T = 9$; </li><li> Booth $2$, buys candy for $2$, $T = 7$; </li><li> Booth $3$, buys candy for $5$, $T = 2$; </li><li> Booth $1$, buys no candy, not enough money; </li><li> Booth $2$, buys candy for $2$, $T = 0$. </li></ol><p>No candy can be bought later. The total number of candies bought is $10$.</p><p>In the second example he has $1$ burle left at the end of his path, no candy can be bought with this amount.</p>
