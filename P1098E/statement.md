## Description

<div><p>Fedya loves problems involving data structures. Especially ones about different queries on subsegments. Fedya had a nice array $a_1, a_2, \ldots a_n$ and a beautiful data structure. This data structure, given $l$ and $r$, $1 \le l \le r \le n$, could find the greatest integer $d$, such that $d$ divides each of $a_l$, $a_{l+1}$, ..., $a_{r}$. </p><p>Fedya really likes this data structure, so he applied it to every non-empty contiguous subarray of array $a$, put all answers into the array and sorted it. He called this array $b$. It's easy to see that array $b$ contains $n(n+1)/2$ elements.</p><p>After that, Fedya implemented another cool data structure, that allowed him to find sum $b_l + b_{l+1} + \ldots + b_r$ for given $l$ and $r$, $1 \le l \le r \le n(n+1)/2$. Surely, Fedya applied this data structure to every contiguous subarray of array $b$, called the result $c$ and sorted it. Help Fedya find the lower median of array $c$.</p><p>Recall that for a sorted array of length $k$ the <span class="tex-font-style-it">lower median</span> is an element at position $\lfloor \frac{k + 1}{2} \rfloor$, if elements of the array are enumerated starting from $1$. For example, the lower median of array $(1, 1, 2, 3, 6)$ is $2$, and the lower median of $(0, 17, 23, 96)$ is $17$.</p></div><div class="input-specification"><p>First line contains a single integer $n$&nbsp;— number of elements in array $a$ ($1 \le n \le 50\,000$). </p><p>Second line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— elements of the array ($1 \le a_i \le 100\,000$).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the lower median of array $c$.</p></div>

## Input

<p>First line contains a single integer $n$&nbsp;— number of elements in array $a$ ($1 \le n \le 50\,000$). </p><p>Second line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— elements of the array ($1 \le a_i \le 100\,000$).</p>

## Output

<p>Print a single integer&nbsp;— the lower median of array $c$.</p>





```input1
2
6 3
```




```input2
2
8 8
```




```input3
5
19 16 2 12 15
```




```output1
6
```




```output2
8
```




```output3
12
```



## Note

<p>In the first sample array $b$ is equal to ${3, 3, 6}$, then array $c$ is equal to ${3, 3, 6, 6, 9, 12}$, so the lower median is $6$.</p><p>In the second sample $b$ is ${8, 8, 8}$, $c$ is ${8, 8, 8, 16, 16, 24}$, so the lower median is $8$.</p>
