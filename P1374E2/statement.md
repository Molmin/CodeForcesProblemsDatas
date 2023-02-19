## Description

<div><p><span class="tex-font-style-bf">Easy and hard versions are actually different problems, so read statements of both problems completely and carefully</span>.</p><p>Summer vacation has started so Alice and Bob want to play and joy, but... Their mom doesn't think so. She says that they have to read <span class="tex-font-style-bf">exactly</span> $m$ books before all entertainments. Alice and Bob will read each book <span class="tex-font-style-bf">together</span> to end this exercise faster.</p><p>There are $n$ books in the family library. The $i$-th book is described by three integers: $t_i$ — the amount of time Alice and Bob need to spend to read it, $a_i$ (equals $1$ if Alice likes the $i$-th book and $0$ if not), and $b_i$ (equals $1$ if Bob likes the $i$-th book and $0$ if not).</p><p>So they need to choose <span class="tex-font-style-bf">exactly</span> $m$ books from the given $n$ books in such a way that:</p><ul> <li> Alice likes <span class="tex-font-style-bf">at least</span> $k$ books from the chosen set and Bob likes <span class="tex-font-style-bf">at least</span> $k$ books from the chosen set; </li><li> the total reading time of these $m$ books is <span class="tex-font-style-bf">minimized</span> (they are children and want to play and joy as soon a possible). </li></ul><p>The set they choose is <span class="tex-font-style-bf">the same</span> for both Alice an Bob (it's shared between them) and they read all books <span class="tex-font-style-bf">together</span>, so the total reading time is the sum of $t_i$ over all books that are in the chosen set.</p><p>Your task is to help them and find any suitable set of books or determine that it is impossible to find such a set.</p></div><div class="input-specification"><p>The first line of the input contains three integers $n$, $m$ and $k$ ($1 \le k \le m \le n \le 2 \cdot 10^5$).</p><p>The next $n$ lines contain descriptions of books, one description per line: the $i$-th line contains three integers $t_i$, $a_i$ and $b_i$ ($1 \le t_i \le 10^4$, $0 \le a_i, b_i \le 1$), where:</p><ul> <li> $t_i$ — the amount of time required for reading the $i$-th book; </li><li> $a_i$ equals $1$ if Alice likes the $i$-th book and $0$ otherwise; </li><li> $b_i$ equals $1$ if Bob likes the $i$-th book and $0$ otherwise. </li></ul></div><div class="output-specification"><p>If there is no solution, print only one integer <span class="tex-font-style-tt">-1</span>.</p><p>If the solution exists, print $T$ in the first line — the minimum total reading time of the suitable set of books. In the second line print $m$ distinct integers from $1$ to $n$ in any order — indices of books which are in the set you found.</p><p>If there are several answers, print any of them.</p></div>

## Input

<p>The first line of the input contains three integers $n$, $m$ and $k$ ($1 \le k \le m \le n \le 2 \cdot 10^5$).</p><p>The next $n$ lines contain descriptions of books, one description per line: the $i$-th line contains three integers $t_i$, $a_i$ and $b_i$ ($1 \le t_i \le 10^4$, $0 \le a_i, b_i \le 1$), where:</p><ul> <li> $t_i$ — the amount of time required for reading the $i$-th book; </li><li> $a_i$ equals $1$ if Alice likes the $i$-th book and $0$ otherwise; </li><li> $b_i$ equals $1$ if Bob likes the $i$-th book and $0$ otherwise. </li></ul>

## Output

<p>If there is no solution, print only one integer <span class="tex-font-style-tt">-1</span>.</p><p>If the solution exists, print $T$ in the first line — the minimum total reading time of the suitable set of books. In the second line print $m$ distinct integers from $1$ to $n$ in any order — indices of books which are in the set you found.</p><p>If there are several answers, print any of them.</p>





```input1
6 3 1
6 0 0
11 1 0
9 0 1
21 1 1
10 1 0
8 0 1

```




```input2
6 3 2
6 0 0
11 1 0
9 0 1
21 1 1
10 1 0
8 0 1

```




```output1
24
6 5 1
```




```output2
39
4 6 5
```


