## Description

<div><p>At the big break Nastya came to the school dining room. There are $n$ pupils in the school, numbered from $1$ to $n$. Unfortunately, Nastya came pretty late, so that all pupils had already stood in the queue, i.e. Nastya took the last place in the queue. Of course, it's a little bit sad for Nastya, but she is not going to despond because some pupils in the queue can agree to change places with some other pupils.</p><p>Formally, there are some pairs $u$, $v$ such that if the pupil with number $u$ stands directly in front of the pupil with number $v$, Nastya can ask them and they will change places. </p><p>Nastya asks you to find the maximal number of places in queue she can move forward. </p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 3 \cdot 10^{5}$, $0 \leq m \leq 5 \cdot 10^{5}$)&nbsp;— the number of pupils in the queue and number of pairs of pupils such that the first one agrees to change places with the second one if the first is directly in front of the second.</p><p>The second line contains $n$ integers $p_1$, $p_2$, ..., $p_n$&nbsp;— the initial arrangement of pupils in the queue, from the queue start to its end ($1 \leq p_i \leq n$, $p$ is a permutation of integers from $1$ to $n$). In other words, $p_i$ is the number of the pupil who stands on the $i$-th position in the queue.</p><p>The $i$-th of the following $m$ lines contains two integers $u_i$, $v_i$ ($1 \leq u_i, v_i \leq n, u_i \neq v_i$), denoting that the pupil with number $u_i$ agrees to change places with the pupil with number $v_i$ if $u_i$ is directly in front of $v_i$. It is guaranteed that if $i \neq j$, than $v_i \neq v_j$ or $u_i \neq u_j$. Note that it is possible that in some pairs both pupils agree to change places with each other.</p><p>Nastya is the last person in the queue, i.e. the pupil with number $p_n$.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of places in queue she can move forward.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 3 \cdot 10^{5}$, $0 \leq m \leq 5 \cdot 10^{5}$)&nbsp;— the number of pupils in the queue and number of pairs of pupils such that the first one agrees to change places with the second one if the first is directly in front of the second.</p><p>The second line contains $n$ integers $p_1$, $p_2$, ..., $p_n$&nbsp;— the initial arrangement of pupils in the queue, from the queue start to its end ($1 \leq p_i \leq n$, $p$ is a permutation of integers from $1$ to $n$). In other words, $p_i$ is the number of the pupil who stands on the $i$-th position in the queue.</p><p>The $i$-th of the following $m$ lines contains two integers $u_i$, $v_i$ ($1 \leq u_i, v_i \leq n, u_i \neq v_i$), denoting that the pupil with number $u_i$ agrees to change places with the pupil with number $v_i$ if $u_i$ is directly in front of $v_i$. It is guaranteed that if $i \neq j$, than $v_i \neq v_j$ or $u_i \neq u_j$. Note that it is possible that in some pairs both pupils agree to change places with each other.</p><p>Nastya is the last person in the queue, i.e. the pupil with number $p_n$.</p>

## Output

<p>Print a single integer&nbsp;— the number of places in queue she can move forward.</p>





```input1
2 1
1 2
1 2

```




```input2
3 3
3 1 2
1 2
3 1
3 2

```




```input3
5 2
3 1 5 4 2
5 2
5 4

```




```output1
1
```




```output2
2
```




```output3
1
```



## Note

<p>In the first example Nastya can just change places with the first pupil in the queue.</p><p>Optimal sequence of changes in the second example is </p><ul> <li> change places for pupils with numbers $1$ and $3$. </li><li> change places for pupils with numbers $3$ and $2$. </li><li> change places for pupils with numbers $1$ and $2$. </li></ul><p>The queue looks like $[3, 1, 2]$, then $[1, 3, 2]$, then $[1, 2, 3]$, and finally $[2, 1, 3]$ after these operations.</p>
