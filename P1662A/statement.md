## Description

<div><p>Gianni, SWERC's chief judge, received a huge amount of high quality problems from the judges and now he has to choose a problem set for SWERC.</p><p>He received $n$ problems and he assigned a beauty score and a difficulty to each of them. The $i$-th problem has beauty score equal to $b_i$ and difficulty equal to $d_i$. The beauty and the difficulty are integers between $1$ and $10$. </p><p>If there are no problems with a certain difficulty (the possible difficulties are $1,2,\dots,10$) then Gianni will ask for more problems to the judges.</p><p>Otherwise, for each difficulty between $1$ and $10$, he will put in the problem set one of the most beautiful problems with such difficulty (so the problem set will contain exactly $10$ problems with distinct difficulties). You shall compute the total beauty of the problem set, that is the sum of the beauty scores of the problems chosen by Gianni.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains the integer $n$ ($1\le n\le 100$) — how many problems Gianni received from the judges.</p><p>The next $n$ lines contain two integers each. The $i$-th of such lines contains $b_i$ and $d_i$ ($1\le b_i, d_i\le 10$) — the beauty score and the difficulty of the $i$-th problem.</p></div><div class="output-specification"><p>For each test case, print the total beauty of the problem set chosen by Gianni. If Gianni cannot create a problem set (because there are no problems with a certain difficulty) print the string <span class="tex-font-style-tt">MOREPROBLEMS</span> (all letters are uppercase, there are no spaces).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains the integer $n$ ($1\le n\le 100$) — how many problems Gianni received from the judges.</p><p>The next $n$ lines contain two integers each. The $i$-th of such lines contains $b_i$ and $d_i$ ($1\le b_i, d_i\le 10$) — the beauty score and the difficulty of the $i$-th problem.</p>

## Output

<p>For each test case, print the total beauty of the problem set chosen by Gianni. If Gianni cannot create a problem set (because there are no problems with a certain difficulty) print the string <span class="tex-font-style-tt">MOREPROBLEMS</span> (all letters are uppercase, there are no spaces).</p>





```input1|2,3,4,5
2
3
8 4
9 3
6 7
12
3 10
10 1
10 2
10 3
10 4
3 10
10 5
10 6
10 7
10 8
10 9
1 10
```




```output1
MOREPROBLEMS
93
```



## Note

<p>In the <span class="tex-font-style-bf">first test case</span>, Gianni has received only $3$ problems, with difficulties $3, 4, 7$ which are not sufficient to create a problem set (for example because there is not a problem with difficulty $1$).</p><p>In the <span class="tex-font-style-bf">second test case</span>, Gianni will create a problem set by taking the problems $2$, $3$, $4$, $5$, $7$, $8$, $9$, $10$, $11$ (which have beauty equal to $10$ and all difficulties from $1$ to $9$) and one of the problems $1$ and $6$ (which have both beauty $3$ and difficulty $10$). The total beauty of the resulting problem set is $10\cdot 9 + 3 = 93$.</p>
