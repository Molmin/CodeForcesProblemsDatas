## Description

<div><p>A sequence $a_1, a_2, \dots, a_n$ is called good if, for each element $a_i$, there exists an element $a_j$ ($i \ne j$) such that $a_i+a_j$ is a power of two (that is, $2^d$ for some non-negative integer $d$).</p><p>For example, the following sequences are good:</p><ul> <li> $[5, 3, 11]$ (for example, for $a_1=5$ we can choose $a_2=3$. Note that their sum is a power of two. Similarly, such an element can be found for $a_2$ and $a_3$), </li><li> $[1, 1, 1, 1023]$, </li><li> $[7, 39, 89, 25, 89]$, </li><li> $[]$. </li></ul><p>Note that, by definition, an empty sequence (with a length of $0$) is good.</p><p>For example, the following sequences are not good:</p><ul> <li> $[16]$ (for $a_1=16$, it is impossible to find another element $a_j$ such that their sum is a power of two), </li><li> $[4, 16]$ (for $a_1=4$, it is impossible to find another element $a_j$ such that their sum is a power of two), </li><li> $[1, 3, 2, 8, 8, 8]$ (for $a_3=2$, it is impossible to find another element $a_j$ such that their sum is a power of two). </li></ul><p>You are given a sequence $a_1, a_2, \dots, a_n$. What is the minimum number of elements you need to remove to make it good? You can delete an arbitrary set of elements.</p></div><div class="input-specification"><p>The first line contains the integer $n$ ($1 \le n \le 120000$) — the length of the given sequence.</p><p>The second line contains the sequence of integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>Print the minimum number of elements needed to be removed from the given sequence in order to make it good. It is possible that you need to delete all $n$ elements, make it empty, and thus get a good sequence.</p></div>

## Input

<p>The first line contains the integer $n$ ($1 \le n \le 120000$) — the length of the given sequence.</p><p>The second line contains the sequence of integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p>

## Output

<p>Print the minimum number of elements needed to be removed from the given sequence in order to make it good. It is possible that you need to delete all $n$ elements, make it empty, and thus get a good sequence.</p>





```input1
6
4 7 1 5 4 9

```




```input2
5
1 2 3 4 5

```




```input3
1
16

```




```input4
4
1 1 1 1023

```




```output1
1

```




```output2
2

```




```output3
1

```




```output4
0

```



## Note

<p>In the first example, it is enough to delete one element $a_4=5$. The remaining elements form the sequence $[4, 7, 1, 4, 9]$, which is good.</p>
