## Description

<div><p>Monocarp is the coach of the Berland State University programming teams. He decided to compose a problemset for a training session for his teams.</p><p>Monocarp has $n$ problems that none of his students have seen yet. The $i$-th problem has a topic $a_i$ (an integer from $1$ to $n$) and a difficulty $b_i$ (an integer from $1$ to $n$). All problems are different, that is, there are no two tasks that have the same topic and difficulty at the same time.</p><p>Monocarp decided to select exactly $3$ problems from $n$ problems for the problemset. The problems should satisfy <span class="tex-font-style-bf">at least one</span> of two conditions (possibly, both):</p><ul> <li> the topics of all three selected problems are different; </li><li> the difficulties of all three selected problems are different. </li></ul><p>Your task is to determine the number of ways to select three problems for the problemset.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 50000$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains an integer $n$ ($3 \le n \le 2 \cdot 10^5$) — the number of problems that Monocarp have.</p><p>In the $i$-th of the following $n$ lines, there are two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$)&nbsp;— the topic and the difficulty of the $i$-th problem.</p><p>It is guaranteed that there are no two problems that have the same topic and difficulty at the same time.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print the number of ways to select three training problems that meet either of the requirements described in the statement.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 50000$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains an integer $n$ ($3 \le n \le 2 \cdot 10^5$) — the number of problems that Monocarp have.</p><p>In the $i$-th of the following $n$ lines, there are two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$)&nbsp;— the topic and the difficulty of the $i$-th problem.</p><p>It is guaranteed that there are no two problems that have the same topic and difficulty at the same time.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>Print the number of ways to select three training problems that meet either of the requirements described in the statement.</p>





```input1
2
4
2 4
3 4
2 1
1 3
5
1 5
2 4
3 3
4 2
5 1
```




```output1
3
10
```



## Note

<p>In the first example, you can take the following sets of three problems:</p><ul> <li> problems $1$, $2$, $4$; </li><li> problems $1$, $3$, $4$; </li><li> problems $2$, $3$, $4$. </li></ul><p>Thus, the number of ways is equal to three.</p>
