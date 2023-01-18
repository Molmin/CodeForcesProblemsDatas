## Description

<div><p>Suppose you are given a sequence $S$ of $k$ pairs of integers $(a_1, b_1), (a_2, b_2), \dots, (a_k, b_k)$.</p><p>You can perform the following operations on it:</p><ol> <li> Choose some position $i$ and <span class="tex-font-style-bf">increase</span> $a_i$ by $1$. That can be performed only if there exists at least one such position $j$ that $i \ne j$ and $a_i = a_j$. The cost of this operation is $b_i$; </li><li> Choose some position $i$ and <span class="tex-font-style-bf">decrease</span> $a_i$ by $1$. That can be performed only if there exists at least one such position $j$ that $a_i = a_j + 1$. The cost of this operation is $-b_i$. </li></ol><p>Each operation can be performed arbitrary number of times (possibly zero).</p><p>Let $f(S)$ be minimum possible $x$ such that there exists a sequence of operations with total cost $x$, after which all $a_i$ from $S$ are pairwise distinct. </p><p><span class="tex-font-style-it">Now for the task itself ...</span></p><p>You are given a sequence $P$ consisting of $n$ pairs of integers $(a_1, b_1), (a_2, b_2), \dots, (a_n, b_n)$. All $b_i$ are pairwise distinct. Let $P_i$ be the sequence consisting of the first $i$ pairs of $P$. Your task is to calculate the values of $f(P_1), f(P_2), \dots, f(P_n)$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of pairs in sequence $P$.</p><p>Next $n$ lines contain the elements of $P$: $i$-th of the next $n$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i \le 2 \cdot 10^5$, $1 \le b_i \le n$). It is guaranteed that all values of $b_i$ are pairwise distinct.</p></div><div class="output-specification"><p>Print $n$ integers — the $i$-th number should be equal to $f(P_i)$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of pairs in sequence $P$.</p><p>Next $n$ lines contain the elements of $P$: $i$-th of the next $n$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i \le 2 \cdot 10^5$, $1 \le b_i \le n$). It is guaranteed that all values of $b_i$ are pairwise distinct.</p>

## Output

<p>Print $n$ integers — the $i$-th number should be equal to $f(P_i)$.</p>





```input1
5
1 1
3 3
5 5
4 2
2 4

```




```input2
4
2 4
2 3
2 2
1 1

```




```output1
0
0
0
-5
-16

```




```output2
0
3
7
1

```


