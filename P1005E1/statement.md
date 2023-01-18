## Description

<div><p>You are given a permutation $p_1, p_2, \dots, p_n$. A permutation of length $n$ is a sequence such that each integer between $1$ and $n$ occurs exactly once in the sequence.</p><p>Find the number of pairs of indices $(l, r)$ ($1 \le l \le r \le n$) such that the value of the median of $p_l, p_{l+1}, \dots, p_r$ is exactly the given number $m$.</p><p>The median of a sequence is the value of the element which is in the middle of the sequence after sorting it in non-decreasing order. If the length of the sequence is even, the left of two middle elements is used.</p><p>For example, if $a=[4, 2, 7, 5]$ then its median is $4$ since after sorting the sequence, it will look like $[2, 4, 5, 7]$ and the left of two middle elements is equal to $4$. The median of $[7, 1, 2, 9, 6]$ equals $6$ since after sorting, the value $6$ will be in the middle of the sequence.</p><p>Write a program to find the number of pairs of indices $(l, r)$ ($1 \le l \le r \le n$) such that the value of the median of $p_l, p_{l+1}, \dots, p_r$ is exactly the given number $m$.</p></div><div class="input-specification"><p>The first line contains integers $n$ and $m$ ($1 \le n \le 2\cdot10^5$, $1 \le m \le n$) — the length of the given sequence and the required value of the median.</p><p>The second line contains a permutation $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$). Each integer between $1$ and $n$ occurs in $p$ exactly once.</p></div><div class="output-specification"><p>Print the required number.</p></div>

## Input

<p>The first line contains integers $n$ and $m$ ($1 \le n \le 2\cdot10^5$, $1 \le m \le n$) — the length of the given sequence and the required value of the median.</p><p>The second line contains a permutation $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$). Each integer between $1$ and $n$ occurs in $p$ exactly once.</p>

## Output

<p>Print the required number.</p>





```input1
5 4
2 4 5 3 1

```




```input2
5 5
1 2 3 4 5

```




```input3
15 8
1 15 2 14 3 13 4 8 12 5 11 6 10 7 9

```




```output1
4

```




```output2
1

```




```output3
48

```



## Note

<p>In the first example, the suitable pairs of indices are: $(1, 3)$, $(2, 2)$, $(2, 3)$ and $(2, 4)$.</p>
