## Description

<div><p>You are given a multiset $S$. Over all pairs of subsets $A$ and $B$, such that:</p><ul> <li> $B \subset A$; </li><li> $|B| = |A| - 1$; </li><li> greatest common divisor of all elements in $A$ is equal to one; </li></ul><p>find the sum of $\sum_{x \in A}{x} \cdot \sum_{x \in B}{x}$, modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains one integer $m$ ($1 \le m \le 10^5$): the number of different values in the multiset $S$.</p><p>Each of the next $m$ lines contains two integers $a_i$, $freq_i$ ($1 \le a_i \le 10^5, 1 \le freq_i \le 10^9$). Element $a_i$ appears in the multiset $S$ $freq_i$ times. All $a_i$ are different.</p></div><div class="output-specification"><p>Print the required sum, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains one integer $m$ ($1 \le m \le 10^5$): the number of different values in the multiset $S$.</p><p>Each of the next $m$ lines contains two integers $a_i$, $freq_i$ ($1 \le a_i \le 10^5, 1 \le freq_i \le 10^9$). Element $a_i$ appears in the multiset $S$ $freq_i$ times. All $a_i$ are different.</p>

## Output

<p>Print the required sum, modulo $998\,244\,353$.</p>





```input1
2
1 1
2 1
```




```input2
4
1 1
2 1
3 1
6 1
```




```input3
1
1 5
```




```output1
9
```




```output2
1207
```




```output3
560
```



## Note

<p>A multiset is a set where elements are allowed to coincide. $|X|$ is the cardinality of a set $X$, the number of elements in it.</p><p>$A \subset B$: Set $A$ is a subset of a set $B$.</p><p>In the first example $B=\{1\}, A=\{1,2\}$ and $B=\{2\}, A=\{1, 2\}$ have a product equal to $1\cdot3 + 2\cdot3=9$. Other pairs of $A$ and $B$ don't satisfy the given constraints.</p>
