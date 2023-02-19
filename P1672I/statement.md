## Description

<div><p>You have a permutation $p$ of integers from $1$ to $n$.</p><p>You have a strength of $s$ and will perform the following operation some times:</p><ul> <li> Choose an index $i$ such that $1 \leq i \leq |p|$ and $|i-p_i| \leq s$. </li><li> For all $j$ such that $1 \leq j \leq |p|$ and $p_i&lt;p_j$, update $p_j$ to $p_j-1$. </li><li> Delete the $i$-th element from $p$. Formally, update $p$ to $[p_1,\ldots,p_{i-1},p_{i+1},\ldots,p_n]$. </li></ul><p>It can be shown that no matter what $i$ you have chosen, $p$ will be a permutation of integers from $1$ to $|p|$ after all operations.</p><p>You want to be able to transform $p$ into the empty permutation. Find the minimum strength $s$ that will allow you to do so.</p></div><div class="input-specification"><p>The first line of input contains a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$) &nbsp;— the length of the permutation $p$.</p><p>The second line of input conatains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$) &nbsp;— the elements of the permutation $p$.</p><p>It is guaranteed that all elements in $p$ are distinct.</p></div><div class="output-specification"><p>Print the minimum strength $s$ required.</p></div>

## Input

<p>The first line of input contains a single integer $n$ ($1 \leq n \leq 5 \cdot 10^5$) &nbsp;— the length of the permutation $p$.</p><p>The second line of input conatains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$) &nbsp;— the elements of the permutation $p$.</p><p>It is guaranteed that all elements in $p$ are distinct.</p>

## Output

<p>Print the minimum strength $s$ required.</p>





```input1
3
3 2 1
```




```input2
1
1
```




```input3
10
1 8 4 3 7 10 6 5 9 2
```




```output1
1
```




```output2
0
```




```output3
1
```



## Note

<p>In the first test case, the minimum $s$ required is $1$.</p><p>Here is how we can transform $p$ into the empty permutation with $s=1$: </p><ul> <li> In the first move, you can only choose $i=2$ as choosing any other value of $i$ will result in $|i-p_i| \leq s$ being false. With $i=2$, $p$ will be changed to $[2,1]$. </li><li> In the second move, you choose $i=1$, then $p$ will be changed to $[1]$. </li><li> In the third move, you choose $i=1$, then $p$ will be changed to $[~]$. </li></ul><p>It can be shown that with $s=0$, it is impossible to transform $p$ into the empty permutation.</p>
