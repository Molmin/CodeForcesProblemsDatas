## Description

<div><p>Kate has a set $S$ of $n$ integers $\{1, \dots, n\} $. </p><p>She thinks that <span class="tex-font-style-bf">imperfection</span> of a subset $M \subseteq S$ is equal to the <span class="tex-font-style-bf">maximum</span> of $gcd(a, b)$ over all pairs $(a, b)$ such that both $a$ and $b$ are in $M$ and $a \neq b$. </p><p>Kate is a very neat girl and for each $k \in \{2, \dots, n\}$ she wants to find a subset that has the <span class="tex-font-style-bf">smallest imperfection</span> among all subsets in $S$ of size $k$. There can be more than one subset with the smallest imperfection and the same size, but you don't need to worry about it. Kate wants to find all the subsets herself, but she needs your help to find the smallest possible imperfection for each size $k$, will name it $I_k$. </p><p>Please, help Kate to find $I_2$, $I_3$, ..., $I_n$.</p></div><div class="input-specification"><p>The first and only line in the input consists of only one integer $n$ ($2\le n \le 5 \cdot 10^5$) &nbsp;— the size of the given set $S$.</p></div><div class="output-specification"><p>Output contains only one line that includes $n - 1$ integers: $I_2$, $I_3$, ..., $I_n$.</p></div>

## Input

<p>The first and only line in the input consists of only one integer $n$ ($2\le n \le 5 \cdot 10^5$) &nbsp;— the size of the given set $S$.</p>

## Output

<p>Output contains only one line that includes $n - 1$ integers: $I_2$, $I_3$, ..., $I_n$.</p>





```input1
2
```




```input2
3
```




```output1
1
```




```output2
1 1
```



## Note

<p>First sample: answer is 1, because $gcd(1, 2) = 1$.</p><p>Second sample: there are subsets of $S$ with sizes $2, 3$ with imperfection equal to 1. For example, $\{2,3\}$ and $\{1, 2, 3\}$.</p>
