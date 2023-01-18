## Description

<div><p>You are given an integer sequence $a_1, a_2, \dots, a_n$.</p><p>Find the number of pairs of indices $(l, r)$ ($1 \le l \le r \le n$) such that the value of median of $a_l, a_{l+1}, \dots, a_r$ is exactly the given number $m$.</p><p>The median of a sequence is the value of an element which is in the middle of the sequence after sorting it in non-decreasing order. If the length of the sequence is even, the left of two middle elements is used.</p><p>For example, if $a=[4, 2, 7, 5]$ then its median is $4$ since after sorting the sequence, it will look like $[2, 4, 5, 7]$ and the left of two middle elements is equal to $4$. The median of $[7, 1, 2, 9, 6]$ equals $6$ since after sorting, the value $6$ will be in the middle of the sequence.</p><p>Write a program to find the number of pairs of indices $(l, r)$ ($1 \le l \le r \le n$) such that the value of median of $a_l, a_{l+1}, \dots, a_r$ is exactly the given number $m$.</p></div><div class="input-specification"><p>The first line contains integers $n$ and $m$ ($1 \le n,m \le 2\cdot10^5$) — the length of the given sequence and the required value of the median.</p><p>The second line contains an integer sequence $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2\cdot10^5$).</p></div><div class="output-specification"><p>Print the required number.</p></div>

## Input

<p>The first line contains integers $n$ and $m$ ($1 \le n,m \le 2\cdot10^5$) — the length of the given sequence and the required value of the median.</p><p>The second line contains an integer sequence $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2\cdot10^5$).</p>

## Output

<p>Print the required number.</p>





```input1
5 4
1 4 5 60 4

```




```input2
3 1
1 1 1

```




```input3
15 2
1 2 3 1 2 3 1 2 3 1 2 3 1 2 3

```




```output1
8

```




```output2
6

```




```output3
97

```



## Note

<p>In the first example, the suitable pairs of indices are: $(1, 3)$, $(1, 4)$, $(1, 5)$, $(2, 2)$, $(2, 3)$, $(2, 5)$, $(4, 5)$ and $(5, 5)$.</p>
