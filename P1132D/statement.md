## Description

<div><p>Berland SU holds yet another training contest for its students today. $n$ students came, each of them brought his laptop. However, it turned out that everyone has forgot their chargers!</p><p>Let students be numbered from $1$ to $n$. Laptop of the $i$-th student has charge $a_i$ at the beginning of the contest and it uses $b_i$ of charge per minute (i.e. if the laptop has $c$ charge at the beginning of some minute, it becomes $c - b_i$ charge at the beginning of the next minute). The whole contest lasts for $k$ minutes.</p><p>Polycarp (the coach of Berland SU) decided to buy a <span class="tex-font-style-bf">single</span> charger so that all the students would be able to successfully finish the contest. He buys the charger at the same moment the contest starts.</p><p>Polycarp can choose to buy the charger with any non-negative (zero or positive) integer power output. The power output is chosen before the purchase, it can't be changed afterwards. Let the chosen power output be $x$. <span class="tex-font-style-bf">At the beginning of each minute</span> (from the minute contest starts to the last minute of the contest) he can plug the charger into any of the student's laptops and use it for some <span class="tex-font-style-bf">integer</span> number of minutes. If the laptop is using $b_i$ charge per minute then it will become $b_i - x$ per minute while the charger is plugged in. Negative power usage rate means that the laptop's charge is increasing. The charge of any laptop isn't limited, it can become infinitely large. The charger can be plugged in no more than one laptop at the same time.</p><p>The student successfully finishes the contest if the charge of his laptop never is below zero at the beginning of some minute (from the minute contest starts to the last minute of the contest, zero charge is allowed). The charge of the laptop of the minute the contest ends doesn't matter.</p><p>Help Polycarp to determine the minimal possible power output the charger should have so that all the students are able to successfully finish the contest. Also report if no such charger exists.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \le k \le 2 \cdot 10^5$) — the number of students (and laptops, correspondigly) and the duration of the contest in minutes.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^{12}$) — the initial charge of each student's laptop.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^7$) — the power usage of each student's laptop.</p></div><div class="output-specification"><p>Print a single non-negative integer — the minimal possible power output the charger should have so that all the students are able to successfully finish the contest.</p><p>If no such charger exists, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \le k \le 2 \cdot 10^5$) — the number of students (and laptops, correspondigly) and the duration of the contest in minutes.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^{12}$) — the initial charge of each student's laptop.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^7$) — the power usage of each student's laptop.</p>

## Output

<p>Print a single non-negative integer — the minimal possible power output the charger should have so that all the students are able to successfully finish the contest.</p><p>If no such charger exists, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
2 4
3 2
4 2
```




```input2
1 5
4
2
```




```input3
1 6
4
2
```




```input4
2 2
2 10
3 15
```




```output1
5
```




```output2
1
```




```output3
2
```




```output4
-1
```



## Note

<p>Let's take a look at the state of laptops in the beginning of each minute on the first example with the charger of power $5$:</p><ol> <li> charge: $[3, 2]$, plug the charger into laptop 1; </li><li> charge: $[3 - 4 + 5, 2 - 2] = [4, 0]$, plug the charger into laptop 2; </li><li> charge: $[4 - 4, 0 - 2 + 5] = [0, 3]$, plug the charger into laptop 1; </li><li> charge: $[0 - 4 + 5, 3 - 2] = [1, 1]$. </li></ol><p>The contest ends after the fourth minute.</p><p>However, let's consider the charger of power $4$:</p><ol> <li> charge: $[3, 2]$, plug the charger into laptop 1; </li><li> charge: $[3 - 4 + 4, 2 - 2] = [3, 0]$, plug the charger into laptop 2; </li><li> charge: $[3 - 4, 0 - 2 + 4] = [-1, 2]$, the first laptop has negative charge, thus, the first student doesn't finish the contest. </li></ol><p>In the fourth example no matter how powerful the charger is, one of the students won't finish the contest.</p>
