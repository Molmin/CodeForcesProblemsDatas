## Description

<div><p>Mishka got an integer array $a$ of length $n$ as a birthday present (what a surprise!).</p><p>Mishka doesn't like this present and wants to change it somehow. He has invented an algorithm and called it "Mishka's Adjacent Replacements Algorithm". This algorithm can be represented as a sequence of steps:</p><ul> <li> Replace each occurrence of $1$ in the array $a$ with $2$; </li><li> Replace each occurrence of $2$ in the array $a$ with $1$; </li><li> Replace each occurrence of $3$ in the array $a$ with $4$; </li><li> Replace each occurrence of $4$ in the array $a$ with $3$; </li><li> Replace each occurrence of $5$ in the array $a$ with $6$; </li><li> Replace each occurrence of $6$ in the array $a$ with $5$; </li><li> $\dots$ </li><li> Replace each occurrence of $10^9 - 1$ in the array $a$ with $10^9$; </li><li> Replace each occurrence of $10^9$ in the array $a$ with $10^9 - 1$. </li></ul><p>Note that the dots in the middle of this algorithm mean that Mishka applies these replacements for each pair of adjacent integers ($2i - 1, 2i$) for each $i \in\{1, 2, \ldots, 5 \cdot 10^8\}$ as described above.</p><p>For example, for the array $a = [1, 2, 4, 5, 10]$, the following sequence of arrays represents the algorithm: </p><p>$[1, 2, 4, 5, 10]$ $\rightarrow$ (replace all occurrences of $1$ with $2$) $\rightarrow$ $[2, 2, 4, 5, 10]$ $\rightarrow$ (replace all occurrences of $2$ with $1$) $\rightarrow$ $[1, 1, 4, 5, 10]$ $\rightarrow$ (replace all occurrences of $3$ with $4$) $\rightarrow$ $[1, 1, 4, 5, 10]$ $\rightarrow$ (replace all occurrences of $4$ with $3$) $\rightarrow$ $[1, 1, 3, 5, 10]$ $\rightarrow$ (replace all occurrences of $5$ with $6$) $\rightarrow$ $[1, 1, 3, 6, 10]$ $\rightarrow$ (replace all occurrences of $6$ with $5$) $\rightarrow$ $[1, 1, 3, 5, 10]$ $\rightarrow$ $\dots$ $\rightarrow$ $[1, 1, 3, 5, 10]$ $\rightarrow$ (replace all occurrences of $10$ with $9$) $\rightarrow$ $[1, 1, 3, 5, 9]$. The later steps of the algorithm do not change the array.</p><p>Mishka is very lazy and he doesn't want to apply these changes by himself. But he is very interested in their result. Help him find it.</p></div><div class="input-specification"><p>The first line of the input contains one integer number $n$ ($1 \le n \le 1000$) — the number of elements in Mishka's birthday present (surprisingly, an array).</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) — the elements of the array.</p></div><div class="output-specification"><p>Print $n$ integers — $b_1, b_2, \dots, b_n$, where $b_i$ is the final value of the $i$-th element of the array after applying "Mishka's Adjacent Replacements Algorithm" to the array $a$. Note that you cannot change the order of elements in the array.</p></div>

## Input

<p>The first line of the input contains one integer number $n$ ($1 \le n \le 1000$) — the number of elements in Mishka's birthday present (surprisingly, an array).</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) — the elements of the array.</p>

## Output

<p>Print $n$ integers — $b_1, b_2, \dots, b_n$, where $b_i$ is the final value of the $i$-th element of the array after applying "Mishka's Adjacent Replacements Algorithm" to the array $a$. Note that you cannot change the order of elements in the array.</p>





```input1
5
1 2 4 5 10

```




```input2
10
10000 10 50605065 1 5 89 5 999999999 60506056 1000000000

```




```output1
1 1 3 5 9

```




```output2
9999 9 50605065 1 5 89 5 999999999 60506055 999999999

```



## Note

<p>The first example is described in the problem statement.</p>
