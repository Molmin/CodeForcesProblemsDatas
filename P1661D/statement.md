## Description

<div><p>You are given two arrays: an array $a$ consisting of $n$ zeros and an array $b$ consisting of $n$ integers.</p><p>You can apply the following operation to the array $a$ an arbitrary number of times: choose some subsegment of $a$ of length $k$ and add the arithmetic progression $1, 2, \ldots, k$ to this subsegment — i. e. add $1$ to the first element of the subsegment, $2$ to the second element, and so on. The chosen subsegment should be inside the borders of the array $a$ (i.e., if the left border of the chosen subsegment is $l$, then the condition $1 \le l \le l + k - 1 \le n$ should be satisfied). Note that the progression added is always $1, 2, \ldots, k$ but not the $k, k - 1, \ldots, 1$ or anything else (i.e., the leftmost element of the subsegment always increases by $1$, the second element always increases by $2$ and so on).</p><p>Your task is to find the <span class="tex-font-style-bf">minimum</span> possible number of operations required to satisfy the condition $a_i \ge b_i$ for each $i$ from $1$ to $n$. Note that the condition $a_i \ge b_i$ should be satisfied for all elements at once.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 3 \cdot 10^5$) — the number of elements in both arrays and the length of the subsegment, respectively.</p><p>The second line of the input contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 10^{12}$), where $b_i$ is the $i$-th element of the array $b$.</p></div><div class="output-specification"><p>Print one integer — the <span class="tex-font-style-bf">minimum</span> possible number of operations required to satisfy the condition $a_i \ge b_i$ for each $i$ from $1$ to $n$.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 3 \cdot 10^5$) — the number of elements in both arrays and the length of the subsegment, respectively.</p><p>The second line of the input contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 10^{12}$), where $b_i$ is the $i$-th element of the array $b$.</p>

## Output

<p>Print one integer — the <span class="tex-font-style-bf">minimum</span> possible number of operations required to satisfy the condition $a_i \ge b_i$ for each $i$ from $1$ to $n$.</p>





```input1
3 3
5 4 6
```




```input2
6 3
1 2 3 2 2 3
```




```input3
6 3
1 2 4 1 2 3
```




```input4
7 3
50 17 81 25 42 39 96
```




```output1
5
```




```output2
3
```




```output3
3
```




```output4
92
```



## Note

<p>Consider the first example. In this test, we don't really have any choice, so we need to add at least five progressions to make the first element equals $5$. The array $a$ becomes $[5, 10, 15]$.</p><p>Consider the second example. In this test, let's add one progression on the segment $[1; 3]$ and two progressions on the segment $[4; 6]$. Then, the array $a$ becomes $[1, 2, 3, 2, 4, 6]$.</p>
