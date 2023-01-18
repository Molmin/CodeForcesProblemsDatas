## Description

<div><p>Polycarp is practicing his problem solving skill. He has a list of $n$ problems with difficulties $a_1, a_2, \dots, a_n$, respectively. His plan is to practice for exactly $k$ days. Each day he has to solve at least one problem from his list. Polycarp solves the problems in the order they are given in his list, he cannot skip any problem from his list. He has to solve all $n$ problems in exactly $k$ days.</p><p>Thus, each day Polycarp solves a contiguous sequence of (consecutive) problems from the start of the list. He can't skip problems or solve them multiple times. As a result, in $k$ days he will solve all the $n$ problems.</p><p>The <span class="tex-font-style-it">profit</span> of the $j$-th day of Polycarp's practice is the maximum among all the difficulties of problems Polycarp solves during the $j$-th day (i.e. if he solves problems with indices from $l$ to $r$ during a day, then the <span class="tex-font-style-it">profit</span> of the day is $\max\limits_{l \le i \le r}a_i$). The <span class="tex-font-style-it">total profit</span> of his practice is the sum of the <span class="tex-font-style-it">profits</span> over all $k$ days of his practice.</p><p>You want to help Polycarp to get the maximum possible <span class="tex-font-style-it">total profit</span> over all valid ways to solve problems. Your task is to distribute all $n$ problems between $k$ days satisfying the conditions above in such a way, that the <span class="tex-font-style-it">total profit</span> is maximum.</p><p>For example, if $n = 8, k = 3$ and $a = [5, 4, 2, 6, 5, 1, 9, 2]$, one of the possible distributions with maximum <span class="tex-font-style-it">total profit</span> is: $[5, 4, 2], [6, 5], [1, 9, 2]$. Here the <span class="tex-font-style-it">total profit</span> equals $5 + 6 + 9 = 20$.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 2000$) — the number of problems and the number of days, respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2000$) — difficulties of problems in Polycarp's list, in the order they are placed in the list (i.e. in the order Polycarp will solve them).</p></div><div class="output-specification"><p>In the first line of the output print the maximum possible <span class="tex-font-style-it">total profit</span>.</p><p>In the second line print exactly $k$ positive integers $t_1, t_2, \dots, t_k$ ($t_1 + t_2 + \dots + t_k$ must equal $n$), where $t_j$ means the number of problems Polycarp will solve during the $j$-th day in order to achieve the maximum possible <span class="tex-font-style-it">total profit</span> of his practice.</p><p>If there are many possible answers, you may print any of them.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 2000$) — the number of problems and the number of days, respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2000$) — difficulties of problems in Polycarp's list, in the order they are placed in the list (i.e. in the order Polycarp will solve them).</p>

## Output

<p>In the first line of the output print the maximum possible <span class="tex-font-style-it">total profit</span>.</p><p>In the second line print exactly $k$ positive integers $t_1, t_2, \dots, t_k$ ($t_1 + t_2 + \dots + t_k$ must equal $n$), where $t_j$ means the number of problems Polycarp will solve during the $j$-th day in order to achieve the maximum possible <span class="tex-font-style-it">total profit</span> of his practice.</p><p>If there are many possible answers, you may print any of them.</p>





```input1
8 3
5 4 2 6 5 1 9 2

```




```input2
5 1
1 1 1 1 1

```




```input3
4 2
1 2000 2000 2

```




```output1
20
3 2 3
```




```output2
1
5

```




```output3
4000
2 2

```



## Note

<p>The first example is described in the problem statement.</p><p>In the second example there is only one possible distribution.</p><p>In the third example the best answer is to distribute problems in the following way: $[1, 2000], [2000, 2]$. The <span class="tex-font-style-it">total profit</span> of this distribution is $2000 + 2000 = 4000$.</p>
