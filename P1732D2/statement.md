## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference is that in this version there are remove queries.</span></p><p>Initially you have a set containing one element — $0$. You need to handle $q$ queries of the following types:</p><ul><li><span class="tex-font-style-tt">+</span> $x$ — add the integer $x$ to the set. It is guaranteed that this integer is not contained in the set;</li><li> <span class="tex-font-style-tt">-</span> $x$ — remove the integer $x$ from the set. It is guaranteed that this integer is contained in the set;</li><li> <span class="tex-font-style-tt">?</span> $k$ — find the $k\text{-mex}$ of the set. </li></ul><p>In our problem, we define the $k\text{-mex}$ of a set of integers as the smallest non-negative integer $x$ that is divisible by $k$ and which is not contained in the set.</p></div><div class="input-specification"><p>The first line contains an integer $q$ ($1 \leq q \leq 2 \cdot 10^5$) — the number of queries.</p><p>The following $q$ lines describe the queries.</p><p>An addition query of integer $x$ is given in the format <span class="tex-font-style-tt">+</span> $x$ ($1 \leq x \leq 10^{18}$). It is guaranteed that $x$ is not contained in the set.</p><p>A remove query of integer $x$ is given in the format <span class="tex-font-style-tt">-</span> $x$ ($1 \leq x \leq 10^{18}$). It is guaranteed that $x$ is contained in the set.</p><p>A search query of $k\text{-mex}$ is given in the format <span class="tex-font-style-tt">?</span> $k$ ($1 \leq k \leq 10^{18}$).</p><p>It is guaranteed that there is at least one query of type <span class="tex-font-style-tt">?</span>.</p></div><div class="output-specification"><p>For each query of type <span class="tex-font-style-tt">?</span> output a single integer — the $k\text{-mex}$ of the set.</p></div>

## Input

<p>The first line contains an integer $q$ ($1 \leq q \leq 2 \cdot 10^5$) — the number of queries.</p><p>The following $q$ lines describe the queries.</p><p>An addition query of integer $x$ is given in the format <span class="tex-font-style-tt">+</span> $x$ ($1 \leq x \leq 10^{18}$). It is guaranteed that $x$ is not contained in the set.</p><p>A remove query of integer $x$ is given in the format <span class="tex-font-style-tt">-</span> $x$ ($1 \leq x \leq 10^{18}$). It is guaranteed that $x$ is contained in the set.</p><p>A search query of $k\text{-mex}$ is given in the format <span class="tex-font-style-tt">?</span> $k$ ($1 \leq k \leq 10^{18}$).</p><p>It is guaranteed that there is at least one query of type <span class="tex-font-style-tt">?</span>.</p>

## Output

<p>For each query of type <span class="tex-font-style-tt">?</span> output a single integer — the $k\text{-mex}$ of the set.</p>





```input1|
18
+ 1
+ 2
? 1
+ 4
? 2
+ 6
? 3
+ 7
+ 8
? 1
? 2
+ 5
? 1
+ 1000000000000000000
? 1000000000000000000
- 4
? 1
? 2
```




```input2|
10
+ 100
? 100
+ 200
? 100
- 100
? 100
+ 50
? 50
- 50
? 50
```




```output1
3
6
3
3
10
3
2000000000000000000
3
4
```




```output2
200
300
100
100
50
```



## Note

<p>In the first example:</p><p>After the first and second queries, the set will contain elements $\{0, 1, 2\}$. The smallest non-negative number that is divisible by $1$ and is not in the set is $3$.</p><p>After the fourth query, the set will contain the elements $\{0, 1, 2, 4\}$. The smallest non-negative number that is divisible by $2$ and is not in the set is $6$.</p><p>In the second example:</p><ul> <li> Initially, the set contains only the element $\{0\}$. </li><li> After adding an integer $100$ the set contains elements $\{0, 100\}$. </li><li> $100\text{-mex}$ of the set is $200$. </li><li> After adding an integer $200$ the set contains elements $\{0, 100, 200\}$. </li><li> $100\text{-mex}$ of the set $300$. </li><li> After removing an integer $100$ the set contains elements $\{0, 200\}$. </li><li> $100\text{-mex}$ of the set is $100$. </li><li> After adding an integer $50$ the set contains elements $\{0, 50, 200\}$. </li><li> $50\text{-mex}$ of the set is $100$. </li><li> After removing an integer $50$ the set contains elements $\{0, 200\}$. </li><li> $100\text{-mex}$ of the set is $50$. </li></ul>
