## Description

<div><p>There are $n$ reindeer at the North Pole, all battling for the highest spot on the "Top Reindeer" leaderboard on the front page of CodeNorses (a popular competitive reindeer gaming website). Interestingly, the "Top Reindeer" title is just a measure of upvotes and has nothing to do with their skill level in the reindeer games, but they still give it the utmost importance.</p><p>Currently, the $i$-th reindeer has a score of $a_i$. You would like to influence the leaderboard with some operations. In an operation, you can choose a reindeer, and either increase or decrease his score by $1$ unit. Negative scores are allowed.</p><p>You have $m$ requirements for the resulting scores. Each requirement is given by an ordered pair $(u, v)$, meaning that after all operations, the score of reindeer $u$ must be less than or equal to the score of reindeer $v$.</p><p>Your task is to perform the minimum number of operations so that all requirements will be satisfied.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2\le n\le 1000$; $1\le m\le 1000$)&nbsp;— the number of reindeer and requirements, respectively.</p><p>The second line contains $n$ integers $a_1,\ldots, a_n$ ($1\le a_i\le 10^9$), where $a_i$ is the current score of reindeer $i$.</p><p>The next $m$ lines describe the requirements.</p><p>The $i$-th of these lines contains two integers $u_i$ and $v_i$ ($1\le u_i, v_i\le n$; $u_i\ne v_i$)&nbsp;— the two reindeer of the $i$-th requirement.</p></div><div class="output-specification"><p>Print $n$ integers $b_1,\ldots, b_n$ ($-10^{15}\le b_i\le 10^{15}$), where $b_i$ is the score of the $i$-th reindeer after all operations.</p><p>If there are multiple solutions achieving the minimum number of operations, you may output any.</p><p>We can prove that there is always an optimal solution such that $|b_i|\le 10^{15}$ for all $i$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2\le n\le 1000$; $1\le m\le 1000$)&nbsp;— the number of reindeer and requirements, respectively.</p><p>The second line contains $n$ integers $a_1,\ldots, a_n$ ($1\le a_i\le 10^9$), where $a_i$ is the current score of reindeer $i$.</p><p>The next $m$ lines describe the requirements.</p><p>The $i$-th of these lines contains two integers $u_i$ and $v_i$ ($1\le u_i, v_i\le n$; $u_i\ne v_i$)&nbsp;— the two reindeer of the $i$-th requirement.</p>

## Output

<p>Print $n$ integers $b_1,\ldots, b_n$ ($-10^{15}\le b_i\le 10^{15}$), where $b_i$ is the score of the $i$-th reindeer after all operations.</p><p>If there are multiple solutions achieving the minimum number of operations, you may output any.</p><p>We can prove that there is always an optimal solution such that $|b_i|\le 10^{15}$ for all $i$.</p>





```input1
7 6
3 1 4 9 2 5 6
1 2
2 3
3 4
4 5
5 6
6 7
```




```input2
4 6
6 5 8 2
3 1
4 1
3 2
1 2
2 3
3 1
```




```input3
10 18
214 204 195 182 180 176 176 172 169 167
1 2
3 2
4 2
5 2
6 2
7 2
8 2
9 2
10 2
6 1
6 2
6 3
6 4
6 5
6 7
6 8
6 9
6 10
```




```output1
1 1 4 4 4 5 6
```




```output2
6 6 6 2
```




```output3
204 204 195 182 180 167 176 172 169 167
```


