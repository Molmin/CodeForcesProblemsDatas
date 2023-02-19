## Description

<div><p>You are organizing a training camp to teach algorithms to young kids. There are $n^2$ kids, organized in an $n$ by $n$ grid. Each kid is between $1$ and $n$ years old (inclusive) and any two kids who are in the same row or in the same column have different ages.</p><p>You want to select exactly $n$ kids for a programming competition, with exactly one kid from each row and one kid from each column. Moreover, kids who are not selected must be either older than both kids selected in their row and column, or younger than both kids selected in their row and column (otherwise they will complain). Notice that it is always possible to select $n$ kids satisfying these requirements (for example by selecting $n$ kids who have the same age).</p><p>During the training camp, you observed that some kids are good at programming, and the others are not. What is the maximum number of kids good at programming that you can select while satisfying all the requirements?</p></div><div class="input-specification"><p>The first line contains $n$ ($1 \leq n \leq 128$) — the size of the grid.</p><p>The following $n$ lines describe the ages of the kids. Specifically, the $i$-th line contains $n$ integers $a_{i,1}, \, a_{i,2}, \, \dots, \, a_{i, n}$ ($1 \le a_{i,j} \le n$) — where $a_{i,j}$ is the age of the kid in the $i$-th row and $j$-th column. It is guaranteed that two kids on the same row or column have different ages, i.e., $a_{i,j} \ne a_{i,j'}$ for any $1\le i\le n$, $1\le j &lt; j'\le n$, and $a_{i,j} \ne a_{i',j}$ for any $1\le i &lt; i'\le n$, $1\le j\le n$.</p><p>The following $n$ lines describe the programming skills of the kids. Specifically, the $i$-th line contains $n$ integers $c_{i,1}, \, c_{i,2}, \, \dots, \, c_{i, n}$ ($c_{i,j} \in \{0, \, 1\}$) — where $c_{i,j}=1$ if the kid in the $i$-th row and $j$-th column is good at programming and $c_{i,j}=0$ otherwise.</p></div><div class="output-specification"><p>Print the maximum number of kids good at programming that you can select while satisfying all the requirements.</p></div>

## Input

<p>The first line contains $n$ ($1 \leq n \leq 128$) — the size of the grid.</p><p>The following $n$ lines describe the ages of the kids. Specifically, the $i$-th line contains $n$ integers $a_{i,1}, \, a_{i,2}, \, \dots, \, a_{i, n}$ ($1 \le a_{i,j} \le n$) — where $a_{i,j}$ is the age of the kid in the $i$-th row and $j$-th column. It is guaranteed that two kids on the same row or column have different ages, i.e., $a_{i,j} \ne a_{i,j'}$ for any $1\le i\le n$, $1\le j &lt; j'\le n$, and $a_{i,j} \ne a_{i',j}$ for any $1\le i &lt; i'\le n$, $1\le j\le n$.</p><p>The following $n$ lines describe the programming skills of the kids. Specifically, the $i$-th line contains $n$ integers $c_{i,1}, \, c_{i,2}, \, \dots, \, c_{i, n}$ ($c_{i,j} \in \{0, \, 1\}$) — where $c_{i,j}=1$ if the kid in the $i$-th row and $j$-th column is good at programming and $c_{i,j}=0$ otherwise.</p>

## Output

<p>Print the maximum number of kids good at programming that you can select while satisfying all the requirements.</p>





```input1
3
1 2 3
3 1 2
2 3 1
1 0 0
0 0 1
0 0 0
```




```input2
4
1 2 3 4
2 1 4 3
3 4 1 2
4 3 2 1
1 1 1 0
0 0 1 0
1 1 0 1
0 0 0 1
```




```output1
1
```




```output2
2
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, it is not possible to select the two kids good at programming (in row $1$ and column $1$, and in row $2$ and column $3$), because then you would have to select the kid in row $3$ and column $2$, and in that case two kids would complain (the one in row $1$ and column $2$, and the one in row $3$ and column $1$).</p><p>A valid selection which contains $1$ kid good at programming is achieved by choosing the $3$ kids who are $1$ year old.</p><p>In the <span class="tex-font-style-bf">second sample</span>, there are $10$ valid choices of the $n$ kids that satisfy the requirements, and each of them selects exactly $2$ kids good at programming.</p>
