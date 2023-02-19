## Description

<div><p>Vanya invented an interesting trick with a set of integers.</p><p>Let an illusionist have a set of positive integers $S$. He names a positive integer $x$. Then an audience volunteer must choose some subset (possibly, empty) of $S$ without disclosing it to the illusionist. The volunteer tells the illusionist the size of the chosen subset. And here comes the trick: the illusionist guesses whether the sum of the subset elements does not exceed $x$. The sum of elements of an empty subset is considered to be $0$.</p><p>Vanya wants to prepare the trick for a public performance. He prepared some set of <span class="tex-font-style-bf">distinct</span> positive integers $S$. Vasya wants the trick to be successful. He calls a positive number $x$ <span class="tex-font-style-it">unsuitable</span>, if he can't be sure that the trick would be successful for every subset a viewer can choose.</p><p>Vanya wants to count the number of unsuitable integers for the chosen set $S$.</p><p>Vanya plans to try different sets $S$. He wants you to write a program that finds the number of unsuitable integers for the initial set $S$, and after each change to the set $S$. Vanya will make $q$ changes to the set, and each change is one of the following two types: </p><ul> <li> add a new integer $a$ to the set $S$, or </li><li> remove some integer $a$ from the set $S$. </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$, $q$ ($1 \leq n, q \leq 200\,000$)&nbsp;— the size of the initial set $S$ and the number of changes.</p><p>The next line contains $n$ <span class="tex-font-style-bf">distinct</span> integers $s_1, s_2, \ldots, s_n$ ($1 \leq s_i \leq 10^{13}$)&nbsp;— the initial elements of $S$.</p><p>Each of the following $q$ lines contain two integers $t_i$, $a_i$ ($1 \leq t_i \leq 2$, $1 \leq a_i \leq 10^{13}$), describing a change: </p><ul> <li> If $t_i = 1$, then an integer $a_i$ is added to the set $S$. It is guaranteed that this integer is not present in $S$ before this operation. </li><li> If $t_i = 2$, then an integer $a_i$ is removed from the set $S$. In is guaranteed that this integer is present in $S$ before this operation. </li></ul></div><div class="output-specification"><p>Print $q + 1$ lines.</p><p>In the first line print the number of unsuitable integers for the initial set $S$. In the next $q$ lines print the number of unsuitable integers for $S$ after each change.</p></div>

## Input

<p>The first line contains two integers $n$, $q$ ($1 \leq n, q \leq 200\,000$)&nbsp;— the size of the initial set $S$ and the number of changes.</p><p>The next line contains $n$ <span class="tex-font-style-bf">distinct</span> integers $s_1, s_2, \ldots, s_n$ ($1 \leq s_i \leq 10^{13}$)&nbsp;— the initial elements of $S$.</p><p>Each of the following $q$ lines contain two integers $t_i$, $a_i$ ($1 \leq t_i \leq 2$, $1 \leq a_i \leq 10^{13}$), describing a change: </p><ul> <li> If $t_i = 1$, then an integer $a_i$ is added to the set $S$. It is guaranteed that this integer is not present in $S$ before this operation. </li><li> If $t_i = 2$, then an integer $a_i$ is removed from the set $S$. In is guaranteed that this integer is present in $S$ before this operation. </li></ul>

## Output

<p>Print $q + 1$ lines.</p><p>In the first line print the number of unsuitable integers for the initial set $S$. In the next $q$ lines print the number of unsuitable integers for $S$ after each change.</p>





```input1
3 11
1 2 3
2 1
1 5
1 6
1 7
2 6
2 2
2 3
1 10
2 5
2 7
2 10
```




```output1
4
1
6
12
19
13
8
2
10
3
0
0
```



## Note

<p>In the first example the initial set is $S = \{1, 2, 3\}$. For this set the trick can be unsuccessful for $x \in \{1, 2, 3, 4\}$. For example, if $x = 4$, the volunteer can choose the subset $\{1, 2\}$ with sum $3 \leq x$, and can choose the subset $\{2, 3\}$ with sum $5 &gt; x$. However, in both cases the illusionist only know the same size of the subset ($2$), so he can't be sure answering making a guess. Since there is only one subset of size $3$, and the sum of each subset of smaller size does not exceed $5$, all $x \ge 5$ are suitable.</p>
