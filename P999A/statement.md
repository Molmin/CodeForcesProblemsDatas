## Description

<div><p>Mishka started participating in a programming contest. There are $n$ problems in the contest. Mishka's problem-solving skill is equal to $k$.</p><p>Mishka arranges all problems from the contest into a list. Because of his weird principles, Mishka only solves problems from one of the ends of the list. Every time, he chooses which end (left or right) he will solve the next problem from. Thus, each problem Mishka solves is either the leftmost or the rightmost problem in the list.</p><p>Mishka cannot solve a problem with difficulty greater than $k$. When Mishka solves the problem, it disappears from the list, so the length of the list decreases by $1$. Mishka stops when he is unable to solve any problem from any end of the list.</p><p>How many problems can Mishka solve?</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $k$ ($1 \le n, k \le 100$) — the number of problems in the contest and Mishka's problem-solving skill.</p><p>The second line of input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the difficulty of the $i$-th problem. The problems are given in order from the leftmost to the rightmost in the list.</p></div><div class="output-specification"><p>Print one integer — the maximum number of problems Mishka can solve.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $k$ ($1 \le n, k \le 100$) — the number of problems in the contest and Mishka's problem-solving skill.</p><p>The second line of input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the difficulty of the $i$-th problem. The problems are given in order from the leftmost to the rightmost in the list.</p>

## Output

<p>Print one integer — the maximum number of problems Mishka can solve.</p>





```input1
8 4
4 2 3 1 5 1 6 4

```




```input2
5 2
3 1 2 1 3

```




```input3
5 100
12 34 55 43 21

```




```output1
5

```




```output2
0

```




```output3
5

```



## Note

<p>In the first example, Mishka can solve problems in the following order: $[4, 2, 3, 1, 5, 1, 6, 4] \rightarrow [2, 3, 1, 5, 1, 6, 4] \rightarrow [2, 3, 1, 5, 1, 6] \rightarrow [3, 1, 5, 1, 6] \rightarrow [1, 5, 1, 6] \rightarrow [5, 1, 6]$, so the number of solved problems will be equal to $5$.</p><p>In the second example, Mishka can't solve any problem because the difficulties of problems from both ends are greater than $k$.</p><p>In the third example, Mishka's solving skill is so amazing that he can solve all the problems.</p>
