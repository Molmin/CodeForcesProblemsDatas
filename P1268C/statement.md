## Description

<div><p>You are given a permutation $p_1, p_2, \ldots, p_n$.</p><p>In one move you can swap two adjacent values.</p><p>You want to perform a minimum number of moves, such that in the end there will exist a subsegment $1,2,\ldots, k$, in other words in the end there should be an integer $i$, $1 \leq i \leq n-k+1$ such that $p_i = 1, p_{i+1} = 2, \ldots, p_{i+k-1}=k$.</p><p>Let $f(k)$ be the minimum number of moves that you need to make a subsegment with values $1,2,\ldots,k$ appear in the permutation.</p><p>You need to find $f(1), f(2), \ldots, f(n)$.</p></div><div class="input-specification"><p>The first line of input contains one integer $n$ ($1 \leq n \leq 200\,000$): the number of elements in the permutation.</p><p>The next line of input contains $n$ integers $p_1, p_2, \ldots, p_n$: given permutation ($1 \leq p_i \leq n$).</p></div><div class="output-specification"><p>Print $n$ integers, the minimum number of moves that you need to make a subsegment with values $1,2,\ldots,k$ appear in the permutation, for $k=1, 2, \ldots, n$.</p></div>

## Input

<p>The first line of input contains one integer $n$ ($1 \leq n \leq 200\,000$): the number of elements in the permutation.</p><p>The next line of input contains $n$ integers $p_1, p_2, \ldots, p_n$: given permutation ($1 \leq p_i \leq n$).</p>

## Output

<p>Print $n$ integers, the minimum number of moves that you need to make a subsegment with values $1,2,\ldots,k$ appear in the permutation, for $k=1, 2, \ldots, n$.</p>





```input1
5
5 4 3 2 1
```




```input2
3
1 2 3
```




```output1
0 1 3 6 10
```




```output2
0 0 0
```


