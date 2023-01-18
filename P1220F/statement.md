## Description

<div><p>Gardener Alex loves to grow trees. We remind that tree is a connected acyclic graph on $n$ vertices. </p><p>Today he decided to grow a rooted binary tree. A binary tree is a tree where any vertex has no more than two sons. Luckily, Alex has a permutation of numbers from $1$ to $n$ which he was presented at his last birthday, so he decided to grow a tree according to this permutation. To do so he does the following process: he finds a minimum element and makes it a root of the tree. After that permutation is divided into two parts: everything that is to the left of the minimum element, and everything that is to the right. The minimum element on the left part becomes the left son of the root, and the minimum element on the right part becomes the right son of the root. After that, this process is repeated recursively on both parts.</p><p>Now Alex wants to grow a forest of trees: one tree for each cyclic shift of the permutation. He is interested in what cyclic shift gives the tree of minimum depth. Unfortunately, growing a forest is a hard and long process, but Alex wants the answer right now. Will you help him?</p><p>We remind that cyclic shift of permutation $a_1, a_2, \ldots, a_k, \ldots, a_n$ for $k$ elements to the left is the permutation $a_{k + 1}, a_{k + 2}, \ldots, a_n, a_1, a_2, \ldots, a_k$.</p></div><div class="input-specification"><p>First line contains an integer number $n ~ (1 \leqslant n \leqslant 200\,000)$ — length of the permutation.</p><p>Second line contains $n$ integer numbers $a_1, a_2, \ldots, a_n ~ (1 \leqslant a_i \leqslant n)$, and it is guaranteed that all numbers occur exactly one time.</p></div><div class="output-specification"><p>Print two numbers separated with space: minimum possible depth of a tree and how many elements we need to shift left to achieve this depth. The number of elements should be a number from $0$ to $n - 1$. If there are several possible answers, print any of them.</p></div>

## Input

<p>First line contains an integer number $n ~ (1 \leqslant n \leqslant 200\,000)$ — length of the permutation.</p><p>Second line contains $n$ integer numbers $a_1, a_2, \ldots, a_n ~ (1 \leqslant a_i \leqslant n)$, and it is guaranteed that all numbers occur exactly one time.</p>

## Output

<p>Print two numbers separated with space: minimum possible depth of a tree and how many elements we need to shift left to achieve this depth. The number of elements should be a number from $0$ to $n - 1$. If there are several possible answers, print any of them.</p>





```input1
4
1 2 3 4
```




```output1
3 2
```



## Note

<p>The following picture depicts all possible trees for sample test and cyclic shifts on which they are achieved. </p><p><img class="tex-graphics" src="file://TFVlU7Ce.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"></p>
