## Description

<div><p>You are given two permutations $a$ and $b$, both of size $n$. A permutation of size $n$ is an array of $n$ elements, where each integer from $1$ to $n$ appears exactly once. The elements in each permutation are indexed from $1$ to $n$.</p><p>You can perform the following operation any number of times:</p><ul> <li> choose an integer $i$ from $1$ to $n$; </li><li> let $x$ be the integer such that $a_x = i$. Swap $a_i$ with $a_x$; </li><li> let $y$ be the integer such that $b_y = i$. Swap $b_i$ with $b_y$. </li></ul><p>Your goal is to make both permutations <span class="tex-font-style-bf">sorted in ascending order</span> (i. e. the conditions $a_1 &lt; a_2 &lt; \dots &lt; a_n$ and $b_1 &lt; b_2 &lt; \dots &lt; b_n$ must be satisfied) using <span class="tex-font-style-bf">minimum number of operations</span>. Note that both permutations must be sorted after you perform the sequence of operations you have chosen.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 3000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$; all $a_i$ are distinct).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le n$; all $b_i$ are distinct).</p></div><div class="output-specification"><p>First, print one integer $k$ ($0 \le k \le 2n$) — the minimum number of operations required to sort both permutations. Note that it can be shown that $2n$ operations are always enough.</p><p>Then, print $k$ integers $op_1, op_2, \dots, op_k$ ($1 \le op_j \le n$), where $op_j$ is the value of $i$ you choose during the $j$-th operation.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 3000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$; all $a_i$ are distinct).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le n$; all $b_i$ are distinct).</p>

## Output

<p>First, print one integer $k$ ($0 \le k \le 2n$) — the minimum number of operations required to sort both permutations. Note that it can be shown that $2n$ operations are always enough.</p><p>Then, print $k$ integers $op_1, op_2, \dots, op_k$ ($1 \le op_j \le n$), where $op_j$ is the value of $i$ you choose during the $j$-th operation.</p><p>If there are multiple answers, print any of them.</p>





```input1
5
1 3 2 4 5
2 1 3 4 5
```




```input2
2
1 2
1 2
```




```input3
4
1 3 4 2
4 3 2 1
```




```output1
1
2
```




```output2
0
```




```output3
2
3 4
```


