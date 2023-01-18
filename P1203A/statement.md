## Description

<div><p>There are $n$ students standing in a circle in some order. The index of the $i$-th student is $p_i$. It is guaranteed that all indices of students are distinct integers from $1$ to $n$ (i. e. they form a permutation).</p><p>Students want to start a round dance. A <span class="tex-font-style-bf">clockwise</span> round dance can be started if the student $2$ comes right after the student $1$ in clockwise order (there are no students between them), the student $3$ comes right after the student $2$ in clockwise order, and so on, and the student $n$ comes right after the student $n - 1$ in clockwise order. A <span class="tex-font-style-bf">counterclockwise</span> round dance is almost the same thing — the only difference is that the student $i$ should be right after the student $i - 1$ in counterclockwise order (this condition should be met for every $i$ from $2$ to $n$). </p><p>For example, if the indices of students listed in clockwise order are $[2, 3, 4, 5, 1]$, then they can start a clockwise round dance. If the students have indices $[3, 2, 1, 4]$ in clockwise order, then they can start a counterclockwise round dance.</p><p>Your task is to determine whether it is possible to start a round dance. Note that the students cannot change their positions before starting the dance; they cannot swap or leave the circle, and no other student can enter the circle. </p><p>You have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 200$) — the number of queries. Then $q$ queries follow.</p><p>The first line of the query contains one integer $n$ ($1 \le n \le 200$) — the number of students.</p><p>The second line of the query contains a permutation of indices $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$), where $p_i$ is the index of the $i$-th student (in clockwise order). It is guaranteed that all $p_i$ are distinct integers from $1$ to $n$ (i. e. they form a permutation).</p></div><div class="output-specification"><p>For each query, print the answer on it. If a round dance can be started with the given order of students, print "<span class="tex-font-style-tt">YES</span>". Otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 200$) — the number of queries. Then $q$ queries follow.</p><p>The first line of the query contains one integer $n$ ($1 \le n \le 200$) — the number of students.</p><p>The second line of the query contains a permutation of indices $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$), where $p_i$ is the index of the $i$-th student (in clockwise order). It is guaranteed that all $p_i$ are distinct integers from $1$ to $n$ (i. e. they form a permutation).</p>

## Output

<p>For each query, print the answer on it. If a round dance can be started with the given order of students, print "<span class="tex-font-style-tt">YES</span>". Otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
5
4
1 2 3 4
3
1 3 2
5
1 2 3 5 4
1
1
5
3 2 1 5 4
```




```output1
YES
YES
NO
YES
YES
```


