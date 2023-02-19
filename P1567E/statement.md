## Description

<div><p>Alice has recently received an array $a_1, a_2, \dots, a_n$ for her birthday! She is very proud of her array, and when she showed her friend Bob the array, he was very happy with her present too!</p><p>However, soon Bob became curious, and as any sane friend would do, asked Alice to perform $q$ operations of two types on her array:</p><ul> <li> $1$ $x$ $y$: update the element $a_x$ to $y$ (set $a_x = y$). </li><li> $2$ $l$ $r$: calculate how many non-decreasing subarrays exist within the subarray $[a_l, a_{l+1}, \dots, a_r]$. More formally, count the number of pairs of integers $(p,q)$ such that $l \le p \le q \le r$ and $a_p \le a_{p+1} \le \dots \le a_{q-1} \le a_q$. </li></ul><p>Help Alice answer Bob's queries!</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;— the size of the array, and the number of queries, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of Alice's array.</p><p>The next $q$ lines consist of three integers each. The first integer of the $i$-th line is $t_i$, the operation being performed on the $i$-th step ($t_i = 1$ or $t_i = 2$).</p><p>If $t_i = 1$, the next two integers are $x_i$ and $y_i$ ($1 \le x_i \le n$; $1 \le y_i \le 10^9$), updating the element at position $x_i$ to $y_i$ (setting $a_{x_i} = y_i$).</p><p>If $t_i = 2$, the next two integers are $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$), the two indices Bob asks Alice about for the $i$-th query.</p><p>It's guaranteed that there is at least one operation of the second type.</p></div><div class="output-specification"><p>For each query of type $2$, print a single integer, the answer to the query.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;— the size of the array, and the number of queries, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of Alice's array.</p><p>The next $q$ lines consist of three integers each. The first integer of the $i$-th line is $t_i$, the operation being performed on the $i$-th step ($t_i = 1$ or $t_i = 2$).</p><p>If $t_i = 1$, the next two integers are $x_i$ and $y_i$ ($1 \le x_i \le n$; $1 \le y_i \le 10^9$), updating the element at position $x_i$ to $y_i$ (setting $a_{x_i} = y_i$).</p><p>If $t_i = 2$, the next two integers are $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$), the two indices Bob asks Alice about for the $i$-th query.</p><p>It's guaranteed that there is at least one operation of the second type.</p>

## Output

<p>For each query of type $2$, print a single integer, the answer to the query.</p>





```input1
5 6
3 1 4 1 5
2 2 5
2 1 3
1 4 4
2 2 5
1 2 6
2 2 5
```




```output1
6
4
10
7
```



## Note

<p>For the first query, $l = 2$ and $r = 5$, and the non-decreasing subarrays $[p,q]$ are $[2,2]$, $[3,3]$, $[4,4]$, $[5,5]$, $[2,3]$ and $[4,5]$.</p>
