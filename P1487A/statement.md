## Description

<div><p>$n$ heroes fight against each other in the Arena. Initially, the $i$-th hero has level $a_i$.</p><p>Each minute, a fight between two different heroes occurs. These heroes can be chosen arbitrarily (<span class="tex-font-style-bf">it's even possible that it is the same two heroes that were fighting during the last minute</span>).</p><p>When two heroes of equal levels fight, nobody wins the fight. When two heroes of different levels fight, the one with the higher level wins, and his level increases by $1$.</p><p>The winner of the tournament is the first hero that wins in at least $100^{500}$ fights <span class="tex-font-style-bf">(note that it's possible that the tournament lasts forever if no hero wins this number of fights, then there is no winner)</span>. A <span class="tex-font-style-it">possible winner</span> is a hero such that there exists a sequence of fights that this hero becomes the winner of the tournament.</p><p>Calculate the number of <span class="tex-font-style-it">possible winners</span> among $n$ heroes.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 500$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains one integer $n$ ($2 \le n \le 100$) — the number of heroes. The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the initial level of the $i$-th hero.</p></div><div class="output-specification"><p>For each test case, print one integer — the number of <span class="tex-font-style-it">possible winners</span> among the given $n$ heroes.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 500$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains one integer $n$ ($2 \le n \le 100$) — the number of heroes. The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the initial level of the $i$-th hero.</p>

## Output

<p>For each test case, print one integer — the number of <span class="tex-font-style-it">possible winners</span> among the given $n$ heroes.</p>





```input1
3
3
3 2 2
2
5 5
4
1 3 3 7
```




```output1
1
0
3
```



## Note

<p>In the first test case of the example, the only <span class="tex-font-style-it">possible winner</span> is the first hero.</p><p>In the second test case of the example, each fight between the heroes results in nobody winning it, so the tournament lasts forever and there is no winner.</p>
