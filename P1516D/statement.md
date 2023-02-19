## Description

<div><p>This time Baby Ehab will only cut and not stick. He starts with a piece of paper with an array $a$ of length $n$ written on it, and then he does the following:</p><ul> <li> he picks a range $(l, r)$ and cuts the subsegment $a_l, a_{l + 1}, \ldots, a_r$ out, removing the rest of the array. </li><li> he then cuts this range into multiple subranges. </li><li> to add a number theory spice to it, he requires that the elements of every subrange must have their product equal to their <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple (LCM)</a>. </li></ul><p>Formally, he partitions the elements of $a_l, a_{l + 1}, \ldots, a_r$ into contiguous subarrays such that the product of every subarray is equal to its LCM. Now, for $q$ independent ranges $(l, r)$, tell Baby Ehab the minimum number of subarrays he needs.</p></div><div class="input-specification"><p>The first line contains $2$ integers $n$ and $q$ ($1 \le n,q \le 10^5$)&nbsp;— the length of the array $a$ and the number of queries.</p><p>The next line contains $n$ integers $a_1$, $a_2$, $\ldots$, $a_n$ ($1 \le a_i \le 10^5$)&nbsp;— the elements of the array $a$.</p><p>Each of the next $q$ lines contains $2$ integers $l$ and $r$ ($1 \le l \le r \le n$)&nbsp;— the endpoints of this query's interval.</p></div><div class="output-specification"><p>For each query, print its answer on a new line.</p></div>

## Input

<p>The first line contains $2$ integers $n$ and $q$ ($1 \le n,q \le 10^5$)&nbsp;— the length of the array $a$ and the number of queries.</p><p>The next line contains $n$ integers $a_1$, $a_2$, $\ldots$, $a_n$ ($1 \le a_i \le 10^5$)&nbsp;— the elements of the array $a$.</p><p>Each of the next $q$ lines contains $2$ integers $l$ and $r$ ($1 \le l \le r \le n$)&nbsp;— the endpoints of this query's interval.</p>

## Output

<p>For each query, print its answer on a new line.</p>





```input1
6 3
2 3 10 7 5 14
1 6
2 4
3 5
```




```output1
3
1
2
```



## Note

<p>The first query asks about the whole array. You can partition it into $[2]$, $[3,10,7]$, and $[5,14]$. The first subrange has product and LCM equal to $2$. The second has product and LCM equal to $210$. And the third has product and LCM equal to $70$. Another possible partitioning is $[2,3]$, $[10,7]$, and $[5,14]$.</p><p>The second query asks about the range $(2,4)$. Its product is equal to its LCM, so you don't need to partition it further.</p><p>The last query asks about the range $(3,5)$. You can partition it into $[10,7]$ and $[5]$.</p>
