## Description

<div><p>Since next season are coming, you'd like to form a team from two or three participants. There are $n$ candidates, the $i$-th candidate has rank $a_i$. But you have weird requirements for your teammates: if you have rank $v$ and have chosen the $i$-th and $j$-th candidate, then $GCD(v, a_i) = X$ and $LCM(v, a_j) = Y$ must be met.</p><p>You are very experienced, so you can change your rank to any non-negative integer but $X$ and $Y$ are tied with your birthdate, so they are fixed.</p><p>Now you want to know, how many are there pairs $(i, j)$ such that there exists an integer $v$ meeting the following constraints: $GCD(v, a_i) = X$ and $LCM(v, a_j) = Y$. It's possible that $i = j$ and you form a team of two.</p><p>$GCD$ is the greatest common divisor of two number, $LCM$ — the least common multiple.</p></div><div class="input-specification"><p>First line contains three integers $n$, $X$ and $Y$ ($1 \le n \le 2 \cdot 10^5$, $1 \le X \le Y \le 10^{18}$) — the number of candidates and corresponding constants.</p><p>Second line contains $n$ space separated integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^{18}$) — ranks of candidates.</p></div><div class="output-specification"><p>Print the only integer — the number of pairs $(i, j)$ such that there exists an integer $v$ meeting the following constraints: $GCD(v, a_i) = X$ and $LCM(v, a_j) = Y$. It's possible that $i = j$.</p></div>

## Input

<p>First line contains three integers $n$, $X$ and $Y$ ($1 \le n \le 2 \cdot 10^5$, $1 \le X \le Y \le 10^{18}$) — the number of candidates and corresponding constants.</p><p>Second line contains $n$ space separated integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^{18}$) — ranks of candidates.</p>

## Output

<p>Print the only integer — the number of pairs $(i, j)$ such that there exists an integer $v$ meeting the following constraints: $GCD(v, a_i) = X$ and $LCM(v, a_j) = Y$. It's possible that $i = j$.</p>





```input1
12 2 2
1 2 3 4 5 6 7 8 9 10 11 12

```




```input2
12 1 6
1 3 5 7 9 11 12 10 8 6 4 2

```




```output1
12

```




```output2
30

```



## Note

<p>In the first example next pairs are valid: $a_j = 1$ and $a_i = [2, 4, 6, 8, 10, 12]$ or $a_j = 2$ and $a_i = [2, 4, 6, 8, 10, 12]$. The $v$ in both cases can be equal to $2$.</p><p>In the second example next pairs are valid: </p><ul> <li> $a_j = 1$ and $a_i = [1, 5, 7, 11]$; </li><li> $a_j = 2$ and $a_i = [1, 5, 7, 11, 10, 8, 4, 2]$; </li><li> $a_j = 3$ and $a_i = [1, 3, 5, 7, 9, 11]$; </li><li> $a_j = 6$ and $a_i = [1, 3, 5, 7, 9, 11, 12, 10, 8, 6, 4, 2]$. </li></ul>
