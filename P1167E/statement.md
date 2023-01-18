## Description

<div><p>You are given an array consisting of $n$ integers $a_1, a_2, \dots , a_n$ and an integer $x$. It is guaranteed that for every $i$, $1 \le a_i \le x$.</p><p>Let's denote a function $f(l, r)$ which erases all values such that $l \le a_i \le r$ from the array $a$ and returns the resulting array. For example, if $a = [4, 1, 1, 4, 5, 2, 4, 3]$, then $f(2, 4) = [1, 1, 5]$.</p><p>Your task is to calculate the number of pairs $(l, r)$ such that $1 \le l \le r \le x$ and $f(l, r)$ is sorted in non-descending order. Note that the empty array is also considered sorted.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $x$ ($1 \le n, x \le 10^6$) — the length of array $a$ and the upper limit for its elements, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots a_n$ ($1 \le a_i \le x$).</p></div><div class="output-specification"><p>Print the number of pairs $1 \le l \le r \le x$ such that $f(l, r)$ is sorted in non-descending order.</p></div>

## Input

<p>The first line contains two integers $n$ and $x$ ($1 \le n, x \le 10^6$) — the length of array $a$ and the upper limit for its elements, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots a_n$ ($1 \le a_i \le x$).</p>

## Output

<p>Print the number of pairs $1 \le l \le r \le x$ such that $f(l, r)$ is sorted in non-descending order.</p>





```input1
3 3
2 3 1
```




```input2
7 4
1 3 1 2 2 4 3
```




```output1
4
```




```output2
6
```



## Note

<p>In the first test case correct pairs are $(1, 1)$, $(1, 2)$, $(1, 3)$ and $(2, 3)$.</p><p>In the second test case correct pairs are $(1, 3)$, $(1, 4)$, $(2, 3)$, $(2, 4)$, $(3, 3)$ and $(3, 4)$.</p>
