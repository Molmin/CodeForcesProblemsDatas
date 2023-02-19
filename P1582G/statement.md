## Description

<div><p>Kuzya started going to school. He was given math homework in which he was given an array $a$ of length $n$ and an array of symbols $b$ of length $n$, consisting of symbols '*' and '/'.</p><p>Let's denote a <span class="tex-font-style-it">path of calculations</span> for a segment $[l; r]$ ($1 \le l \le r \le n$) in the following way: </p><ul> <li> Let $x=1$ initially. For every $i$ from $l$ to $r$ we will consequently do the following: if $b_i=$ '*', $x=x*a_i$, and if $b_i=$ '/', then $x=\frac{x}{a_i}$. Let's call <span class="tex-font-style-it">a path of calculations</span> for the segment $[l; r]$ a list of all $x$ that we got during the calculations (the number of them is exactly $r - l + 1$). </li></ul><p>For example, let $a=[7,$ $12,$ $3,$ $5,$ $4,$ $10,$ $9]$, $b=[/,$ $*,$ $/,$ $/,$ $/,$ $*,$ $*]$, $l=2$, $r=6$, then the path of calculations for that segment is $[12,$ $4,$ $0.8,$ $0.2,$ $2]$.</p><p>Let's call a segment $[l;r]$ <span class="tex-font-style-it">simple</span> if the path of calculations for it contains <span class="tex-font-style-bf">only integer numbers</span>. </p><p>Kuzya needs to find the number of simple segments $[l;r]$ ($1 \le l \le r \le n$). Since he obviously has no time and no interest to do the calculations for each option, he asked you to write a program to get to find that number!</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^6$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p><p>The third line contains $n$ symbols without spaces between them — the array $b_1, b_2 \ldots b_n$ ($b_i=$ '/' or $b_i=$ '*' for every $1 \le i \le n$).</p></div><div class="output-specification"><p>Print a single integer — the number of simple segments $[l;r]$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^6$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p><p>The third line contains $n$ symbols without spaces between them — the array $b_1, b_2 \ldots b_n$ ($b_i=$ '/' or $b_i=$ '*' for every $1 \le i \le n$).</p>

## Output

<p>Print a single integer — the number of simple segments $[l;r]$.</p>





```input1
3
1 2 3
*/*
```




```input2
7
6 4 10 1 2 15 1
*/*/*//
```




```output1
2
```




```output2
8
```


