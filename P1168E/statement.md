## Description

<div><p>Toad Mikhail has an array of $2^k$ integers $a_1, a_2, \ldots, a_{2^k}$.</p><p>Find two permutations $p$ and $q$ of integers $0, 1, \ldots, 2^k-1$, such that $a_i$ is equal to $p_i \oplus q_i$ for all possible $i$, or determine there are no such permutations. Here $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p></div><div class="input-specification"><p>The first line contains one integer $k$ ($2 \leq k \leq 12$), denoting that the size of the array is $2^k$.</p><p>The next line contains $2^k$ space-separated integers $a_1, a_2, \ldots, a_{2^k}$ ($0 \leq a_i &lt; 2^k$)&nbsp;— the elements of the given array.</p></div><div class="output-specification"><p>If the given array can't be represented as element-wise XOR of two permutations of integers $0, 1, \ldots, 2^k-1$, print "<span class="tex-font-style-tt">Fou</span>".</p><p>Otherwise, print "<span class="tex-font-style-tt">Shi</span>" in the first line.</p><p>The next two lines should contain the description of two suitable permutations. The first of these lines should contain $2^k$ space-separated distinct integers $p_{1}, p_{2}, \ldots, p_{2^k}$, and the second line should contain $2^k$ space-separated distinct integers $q_{1}, q_{2}, \ldots, q_{2^k}$.</p><p>All elements of $p$ and $q$ should be between $0$ and $2^k - 1$, inclusive; $p_i \oplus q_i$ should be equal to $a_i$ for all $i$ such that $1 \leq i \leq 2^k$. If there are several possible solutions, you can print any.</p></div>

## Input

<p>The first line contains one integer $k$ ($2 \leq k \leq 12$), denoting that the size of the array is $2^k$.</p><p>The next line contains $2^k$ space-separated integers $a_1, a_2, \ldots, a_{2^k}$ ($0 \leq a_i &lt; 2^k$)&nbsp;— the elements of the given array.</p>

## Output

<p>If the given array can't be represented as element-wise XOR of two permutations of integers $0, 1, \ldots, 2^k-1$, print "<span class="tex-font-style-tt">Fou</span>".</p><p>Otherwise, print "<span class="tex-font-style-tt">Shi</span>" in the first line.</p><p>The next two lines should contain the description of two suitable permutations. The first of these lines should contain $2^k$ space-separated distinct integers $p_{1}, p_{2}, \ldots, p_{2^k}$, and the second line should contain $2^k$ space-separated distinct integers $q_{1}, q_{2}, \ldots, q_{2^k}$.</p><p>All elements of $p$ and $q$ should be between $0$ and $2^k - 1$, inclusive; $p_i \oplus q_i$ should be equal to $a_i$ for all $i$ such that $1 \leq i \leq 2^k$. If there are several possible solutions, you can print any.</p>





```input1
2
0 1 2 3
```




```input2
2
0 0 0 0
```




```input3
2
0 1 2 2
```




```output1
Shi
2 0 1 3 
2 1 3 0
```




```output2
Shi
0 1 2 3 
0 1 2 3
```




```output3
Fou
```


