## Description

<div><p>To AmShZ, all arrays are equal, but some arrays are <span class="tex-font-style-bf">more-equal</span> than others. Specifically, the arrays consisting of $n$ elements from $1$ to $n$ that can be turned into permutations of numbers from $1$ to $n$ by adding a non-negative integer to each element.</p><p>Mashtali <span class="tex-font-style-striked">who wants to appear in every problem statement</span> thinks that an array $b$ consisting of $k$ elements is compatible with a <span class="tex-font-style-bf">more-equal</span> array $a$ consisting of $n$ elements if for each $1 \le i \le k$ we have $1 \le b_i \le n$ and also $a_{b_1} = a_{b_2} = \ldots = a_{b_k}$.</p><p>Find the number of pairs of arrays $a$ and $b$ such that $a$ is a more-equal array consisting of $n$ elements and $b$ is an array compatible with $a$ consisting of $k$ elements modulo $998244353$.</p><p>Note that the elements of $b$ are <span class="tex-font-style-bf">not necessarily distinct</span>, same holds for $a$.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $k$ $(1 \le n \le 10^9 , 1 \le k \le 10^5)$.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem modulo $998244353$.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $k$ $(1 \le n \le 10^9 , 1 \le k \le 10^5)$.</p>

## Output

<p>Print a single integer — the answer to the problem modulo $998244353$.</p>





```input1
1 1
```




```input2
2 2
```




```input3
5 4
```




```input4
20 100
```




```input5
10000000 10000
```




```output1
1
```




```output2
8
```




```output3
50400
```




```output4
807645526
```




```output5
883232350
```



## Note

<p>There are eight possible pairs for the second example: </p><ol> <li> $a = \{1, 1\}, b = \{1, 1\}$ </li><li> $a = \{1, 1\}, b = \{1, 2\}$ </li><li> $a = \{1, 1\}, b = \{2, 1\}$ </li><li> $a = \{1, 1\}, b = \{2, 2\}$ </li><li> $a = \{1, 2\}, b = \{1, 1\}$ </li><li> $a = \{1, 2\}, b = \{2, 2\}$ </li><li> $a = \{2, 1\}, b = \{1, 1\}$ </li><li> $a = \{2, 1\}, b = \{2, 2\}$ </li></ol>
