## Description

<div><p>You are the gym teacher in the school.</p><p>There are $n$ students in the row. And there are two rivalling students among them. The first one is in position $a$, the second in position $b$. Positions are numbered from $1$ to $n$ from left to right.</p><p>Since they are rivals, you want to maximize the distance between them. If students are in positions $p$ and $s$ respectively, then distance between them is $|p - s|$. </p><p>You can do the following operation at most $x$ times: choose two <span class="tex-font-style-bf">adjacent (neighbouring)</span> students and swap them.</p><p>Calculate the maximum distance between two rivalling students after at most $x$ swaps.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The only line of each test case contains four integers $n$, $x$, $a$ and $b$ ($2 \le n \le 100$, $0 \le x \le 100$, $1 \le a, b \le n$, $a \neq b$) — the number of students in the row, the number of swaps which you can do, and positions of first and second rivaling students respectively.</p></div><div class="output-specification"><p>For each test case print one integer — the maximum distance between two rivaling students which you can obtain.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The only line of each test case contains four integers $n$, $x$, $a$ and $b$ ($2 \le n \le 100$, $0 \le x \le 100$, $1 \le a, b \le n$, $a \neq b$) — the number of students in the row, the number of swaps which you can do, and positions of first and second rivaling students respectively.</p>

## Output

<p>For each test case print one integer — the maximum distance between two rivaling students which you can obtain.</p>





```input1
3
5 1 3 2
100 33 100 1
6 0 2 3
```




```output1
2
99
1
```



## Note

<p>In the first test case you can swap students in positions $3$ and $4$. And then the distance between the rivals is equal to $|4 - 2| = 2$.</p><p>In the second test case you don't have to swap students. </p><p>In the third test case you can't swap students.</p>
