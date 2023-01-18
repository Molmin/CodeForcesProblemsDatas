## Description

<div><p>Mateusz likes to travel! However, on his $42$nd visit to Saint Computersburg there is not much left to sightsee. That's why he decided to go to an escape room with his friends!</p><p>The team has solved all riddles flawlessly. There is only one riddle remaining — a huge circular table! There are $n$ weighing scales lying on top of the table, distributed along the circle. Each scale is adjacent to exactly two other scales: for each $i \in \{1, 2, \dots, n-1\}$, the $i$-th and the $(i+1)$-th scales are adjacent to each other, as well as the first and the $n$-th scale.</p><p>The $i$-th scale initially contains $a_i$ heavy coins. Mateusz can perform moves — each move consists of fetching a single coin from one scale and putting it on any adjacent scale.</p><p>It turns out that the riddle will be solved when there is a specific amount of coins on each of the scales. Specifically, each scale has parameters $l_i$ and $r_i$. If each coin lies on a single scale and for each $i$, the $i$-th scale contains at least $l_i$ and at most $r_i$ coins, the riddle will be solved and Mateusz's team will win!</p><p>Mateusz is aiming for the best possible time. Therefore, he wants to solved the riddle as quickly as possible. What is the minimum possible number of moves required to fulfill all the conditions?</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($3 \le n \le 35\,000$) — the number of weighing scales in the circle.</p><p>The following $n$ lines describe the scales. The $i$-th of these lines describes the $i$-th scale and consists of three integers $a_i, l_i, r_i$ ($0 \le a_i \le 35\,000$, $0 \le l_i \le r_i \le 35\,000$).</p><p>It's guaranteed that the riddle is solvable, that is, $\sum_{i=1}^n l_i \le \sum_{i=1}^n a_i \le \sum_{i=1}^n r_i$.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the minimum number of operations required to solve the riddle.</p></div>

## Input

<p>The first line contains an integer $n$ ($3 \le n \le 35\,000$) — the number of weighing scales in the circle.</p><p>The following $n$ lines describe the scales. The $i$-th of these lines describes the $i$-th scale and consists of three integers $a_i, l_i, r_i$ ($0 \le a_i \le 35\,000$, $0 \le l_i \le r_i \le 35\,000$).</p><p>It's guaranteed that the riddle is solvable, that is, $\sum_{i=1}^n l_i \le \sum_{i=1}^n a_i \le \sum_{i=1}^n r_i$.</p>

## Output

<p>Output one integer&nbsp;— the minimum number of operations required to solve the riddle.</p>





```input1
5
0 2 3
1 2 3
4 3 3
4 3 3
4 3 3
```




```input2
3
0 1 2
3 0 3
1 0 0
```




```input3
4
1 0 2
3 3 3
4 0 4
5 3 5
```




```output1
4
```




```output2
1
```




```output3
0
```


