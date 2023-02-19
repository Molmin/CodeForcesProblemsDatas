## Description

<div><p>You may know that Euclid was a mathematician. Well, as it turns out, Morpheus knew it too. So when he wanted to play a mean trick on Euclid, he sent him an appropriate nightmare. </p><p>In his bad dream Euclid has a set $S$ of $n$ $m$-dimensional vectors over the $\mathbb{Z}_2$ field and can perform vector addition on them. In other words he has vectors with $m$ coordinates, each one equal either $0$ or $1$. Vector addition is defined as follows: let $u+v = w$, then $w_i = (u_i + v_i) \bmod 2$. </p><p>Euclid can sum any subset of $S$ and archive another $m$-dimensional vector over $\mathbb{Z}_2$. In particular, he can sum together an empty subset; in such a case, the resulting vector has all coordinates equal $0$.</p><p>Let $T$ be the set of all the vectors that can be written as a sum of some vectors from $S$. Now Euclid wonders the size of $T$ and whether he can use only a subset $S'$ of $S$ to obtain all the vectors from $T$. As it is usually the case in such scenarios, he will not wake up until he figures this out. So far, things are looking rather grim for the philosopher. But there is hope, as he noticed that all vectors in $S$ have <span class="tex-font-style-bf">at most</span> $2$ coordinates equal $1$. </p><p>Help Euclid and calculate $|T|$, the number of $m$-dimensional vectors over $\mathbb{Z}_2$ that can be written as a sum of some vectors from $S$. As it can be quite large, calculate it modulo $10^9+7$. You should also find $S'$, the <span class="tex-font-style-bf">smallest</span> such subset of $S$, that all vectors in $T$ can be written as a sum of vectors from $S'$. In case there are multiple such sets with a minimal number of elements, output the lexicographically smallest one with respect to the order in which their elements are given in the input. </p><p>Consider sets $A$ and $B$ such that $|A| = |B|$. Let $a_1, a_2, \dots a_{|A|}$ and $b_1, b_2, \dots b_{|B|}$ be increasing arrays of indices elements of $A$ and $B$ correspondingly. $A$ is lexicographically smaller than $B$ iff there exists such $i$ that $a_j = b_j$ for all $j &lt; i$ and $a_i &lt; b_i$.</p></div><div class="input-specification"><p>In the first line of input, there are two integers $n$, $m$ ($1 \leq n, m \leq 5 \cdot 10^5$) denoting the number of vectors in $S$ and the number of dimensions. </p><p>Next $n$ lines contain the description of the vectors in $S$. In each of them there is an integer $k$ ($1 \leq k \leq 2$) and then follow $k$ distinct integers $x_1, \dots x_k$ ($1 \leq x_i \leq m$). This encodes an $m$-dimensional vector having $1$s on coordinates $x_1, \dots x_k$ and $0$s on the rest of them.</p><p>Among the $n$ vectors, no two are the same.</p></div><div class="output-specification"><p>In the first line, output two integers: remainder modulo $10^9+7$ of $|T|$ and $|S'|$. In the second line, output $|S'|$ numbers, indices of the elements of $S'$ in ascending order. The elements of $S$ are numbered from $1$ in the order they are given in the input.</p></div>

## Input

<p>In the first line of input, there are two integers $n$, $m$ ($1 \leq n, m \leq 5 \cdot 10^5$) denoting the number of vectors in $S$ and the number of dimensions. </p><p>Next $n$ lines contain the description of the vectors in $S$. In each of them there is an integer $k$ ($1 \leq k \leq 2$) and then follow $k$ distinct integers $x_1, \dots x_k$ ($1 \leq x_i \leq m$). This encodes an $m$-dimensional vector having $1$s on coordinates $x_1, \dots x_k$ and $0$s on the rest of them.</p><p>Among the $n$ vectors, no two are the same.</p>

## Output

<p>In the first line, output two integers: remainder modulo $10^9+7$ of $|T|$ and $|S'|$. In the second line, output $|S'|$ numbers, indices of the elements of $S'$ in ascending order. The elements of $S$ are numbered from $1$ in the order they are given in the input.</p>





```input1
3 2
1 1
1 2
2 2 1
```




```input2
2 3
2 1 3
2 1 2
```




```input3
3 5
2 1 2
1 3
1 4
```




```output1
4 2
1 2
```




```output2
4 2
1 2
```




```output3
8 3
1 2 3
```



## Note

<p>In the first example we are given three vectors: </p><ul> <li> $10$ </li><li> $01$ </li><li> $11$ </li></ul><p>It turns out that we can represent all vectors from our $2$-dimensional space using these vectors: </p><ul> <li> $00$ is a sum of the empty subset of above vectors; </li><li> $01 = 11 + 10$, is a sum of the first and third vector; </li><li> $10 = 10$, is just the first vector; </li><li> $11 = 10 + 01$, is a sum of the first and the second vector. </li></ul><p>Hence, $T = \{00, 01, 10, 11\}$. We can choose any two of the three vectors from $S$ and still be able to obtain all the vectors in $T$. In such a case, we choose the two vectors which appear first in the input. Since we cannot obtain all vectors in $T$ using only a single vector from $S$, $|S'| = 2$ and $S' = \{10, 01\}$ (indices $1$ and $2$), as set $\{1, 2 \}$ is lexicographically the smallest. We can represent all vectors from $T$, using only vectors from $S'$, as shown below: </p><ul> <li> $00$ is a sum of the empty subset; </li><li> $01 = 01$ is just the second vector; </li><li> $10 = 10$ is just the first vector; </li><li> $11 = 10 + 01$ is a sum of the first and the second vector. </li></ul>
