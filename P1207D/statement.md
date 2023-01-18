## Description

<div><p>You are given a sequence of $n$ pairs of integers: $(a_1, b_1), (a_2, b_2), \dots , (a_n, b_n)$. This sequence is called bad if it is sorted in non-descending order by first elements or if it is sorted in non-descending order by second elements. Otherwise the sequence is good. There are examples of good and bad sequences:</p><ul> <li> $s = [(1, 2), (3, 2), (3, 1)]$ is bad because the sequence of first elements is sorted: $[1, 3, 3]$; </li><li> $s = [(1, 2), (3, 2), (1, 2)]$ is bad because the sequence of second elements is sorted: $[2, 2, 2]$; </li><li> $s = [(1, 1), (2, 2), (3, 3)]$ is bad because both sequences (the sequence of first elements and the sequence of second elements) are sorted; </li><li> $s = [(1, 3), (3, 3), (2, 2)]$ is good because neither the sequence of first elements $([1, 3, 2])$ nor the sequence of second elements $([3, 3, 2])$ is sorted. </li></ul><p>Calculate the number of permutations of size $n$ such that after applying this permutation to the sequence $s$ it turns into a good sequence. </p><p>A permutation $p$ of size $n$ is a sequence $p_1, p_2, \dots , p_n$ consisting of $n$ distinct integers from $1$ to $n$ ($1 \le p_i \le n$). If you apply permutation $p_1, p_2, \dots , p_n$ to the sequence $s_1, s_2, \dots , s_n$ you get the sequence $s_{p_1}, s_{p_2}, \dots , s_{p_n}$. For example, if $s = [(1, 2), (1, 3), (2, 3)]$ and $p = [2, 3, 1]$ then $s$ turns into $[(1, 3), (2, 3), (1, 2)]$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 3 \cdot 10^5$).</p><p>The next $n$ lines contains description of sequence $s$. The $i$-th line contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$) — the first and second elements of $i$-th pair in the sequence.</p><p><span class="tex-font-style-bf">The sequence $s$ may contain equal elements</span>.</p></div><div class="output-specification"><p>Print the number of permutations of size $n$ such that after applying this permutation to the sequence $s$ it turns into a good sequence. Print the answer modulo $998244353$ (a prime number).</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 3 \cdot 10^5$).</p><p>The next $n$ lines contains description of sequence $s$. The $i$-th line contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$) — the first and second elements of $i$-th pair in the sequence.</p><p><span class="tex-font-style-bf">The sequence $s$ may contain equal elements</span>.</p>

## Output

<p>Print the number of permutations of size $n$ such that after applying this permutation to the sequence $s$ it turns into a good sequence. Print the answer modulo $998244353$ (a prime number).</p>





```input1
3
1 1
2 2
3 1
```




```input2
4
2 3
2 2
2 1
2 4
```




```input3
3
1 1
1 1
2 3
```




```output1
3
```




```output2
0
```




```output3
4
```



## Note

<p>In first test case there are six permutations of size $3$: </p><ol> <li> if $p = [1, 2, 3]$, then $s = [(1, 1), (2, 2), (3, 1)]$ — bad sequence (sorted by first elements); </li><li> if $p = [1, 3, 2]$, then $s = [(1, 1), (3, 1), (2, 2)]$ — bad sequence (sorted by second elements); </li><li> if $p = [2, 1, 3]$, then $s = [(2, 2), (1, 1), (3, 1)]$ — good sequence; </li><li> if $p = [2, 3, 1]$, then $s = [(2, 2), (3, 1), (1, 1)]$ — good sequence; </li><li> if $p = [3, 1, 2]$, then $s = [(3, 1), (1, 1), (2, 2)]$ — bad sequence (sorted by second elements); </li><li> if $p = [3, 2, 1]$, then $s = [(3, 1), (2, 2), (1, 1)]$ — good sequence. </li></ol>
