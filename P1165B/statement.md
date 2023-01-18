## Description

<div><p>Polycarp wants to train before another programming competition. During the first day of his training he should solve exactly $1$ problem, during the second day — exactly $2$ problems, during the third day — exactly $3$ problems, and so on. During the $k$-th day he should solve $k$ problems.</p><p>Polycarp has a list of $n$ contests, the $i$-th contest consists of $a_i$ problems. During each day Polycarp has to choose <span class="tex-font-style-bf">exactly one</span> of the contests he didn't solve yet and solve it. He solves <span class="tex-font-style-bf">exactly $k$ problems from this contest</span>. Other problems are discarded from it. If there are no contests consisting of at least $k$ problems that Polycarp didn't solve yet during the $k$-th day, then Polycarp stops his training.</p><p>How many days Polycarp can train if he chooses the contests optimally?</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of contests.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$) — the number of problems in the $i$-th contest.</p></div><div class="output-specification"><p>Print one integer — the maximum number of days Polycarp can train if he chooses the contests optimally.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of contests.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$) — the number of problems in the $i$-th contest.</p>

## Output

<p>Print one integer — the maximum number of days Polycarp can train if he chooses the contests optimally.</p>





```input1
4
3 1 4 1
```




```input2
3
1 1 1
```




```input3
5
1 1 1 2 2
```




```output1
3
```




```output2
1
```




```output3
2
```


