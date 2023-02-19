## Description

<div><p>Pak Chanek is given an array $a$ of $n$ integers. For each $i$ ($1 \leq i \leq n$), Pak Chanek will write the one-element set $\{a_i\}$ on a whiteboard.</p><p>After that, in one operation, Pak Chanek may do the following: </p><ol> <li> Choose two different sets $S$ and $T$ on the whiteboard such that $S \cap T = \varnothing$ ($S$ and $T$ do not have any common elements). </li><li> Erase $S$ and $T$ from the whiteboard and write $S \cup T$ (the union of $S$ and $T$) onto the whiteboard. </li></ol><p>After performing zero or more operations, Pak Chanek will construct a multiset $M$ containing the sizes of all sets written on the whiteboard. In other words, each element in $M$ corresponds to the size of a set after the operations.</p><p>How many distinct$^\dagger$ multisets $M$ can be created by this process? Since the answer may be large, output it modulo $998\,244\,353$.</p><p>$^\dagger$ Multisets $B$ and $C$ are different if and only if there exists a value $k$ such that the number of elements with value $k$ in $B$ is different than the number of elements with value $k$ in $C$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$).</p></div><div class="output-specification"><p>Output the number of distinct multisets $M$ modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$).</p>

## Output

<p>Output the number of distinct multisets $M$ modulo $998\,244\,353$.</p>





```input1
6
1 1 2 1 4 3
```




```input2
7
3 5 4 3 7 4 5
```




```output1
7
```




```output2
11
```



## Note

<p>In the first example, the possible multisets $M$ are $\{1,1,1,1,1,1\}$, $\{1,1,1,1,2\}$, $\{1,1,1,3\}$, $\{1,1,2,2\}$, $\{1,1,4\}$, $\{1,2,3\}$, and $\{2,2,2\}$.</p><p>As an example, let's consider a possible sequence of operations. </p><ol> <li> In the beginning, the sets are $\{1\}$, $\{1\}$, $\{2\}$, $\{1\}$, $\{4\}$, and $\{3\}$. </li><li> Do an operation on sets $\{1\}$ and $\{3\}$. Now, the sets are $\{1\}$, $\{1\}$, $\{2\}$, $\{4\}$, and $\{1,3\}$. </li><li> Do an operation on sets $\{2\}$ and $\{4\}$. Now, the sets are $\{1\}$, $\{1\}$, $\{1,3\}$, and $\{2,4\}$. </li><li> Do an operation on sets $\{1,3\}$ and $\{2,4\}$. Now, the sets are $\{1\}$, $\{1\}$, and $\{1,2,3,4\}$. </li><li> The multiset $M$ that is constructed is $\{1,1,4\}$. </li></ol>
