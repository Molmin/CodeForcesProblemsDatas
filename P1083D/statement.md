## Description

<div><p>The Fair Nut has found an array $a$ of $n$ integers. We call subarray $l \ldots r$ a sequence of consecutive elements of an array with indexes from $l$ to $r$, i.e. $a_l, a_{l+1}, a_{l+2}, \ldots, a_{r-1}, a_{r}$. </p><p>No one knows the reason, but he calls a pair of subsegments good if and only if the following conditions are satisfied:</p><ol><li> These subsegments should not be nested. That is, each of the subsegments should contain an element (as an index) that does not belong to another subsegment.</li><li> Subsegments intersect and each element that belongs to the intersection belongs each of segments only once.</li></ol><p>For example $a=[1, 2, 3, 5, 5]$. Pairs $(1 \ldots 3; 2 \ldots 5)$ and $(1 \ldots 2; 2 \ldots 3)$)&nbsp;— are good, but $(1 \dots 3; 2 \ldots 3)$ and $(3 \ldots 4; 4 \ldots 5)$&nbsp;— are not (subsegment $1 \ldots 3$ contains subsegment $2 \ldots 3$, integer $5$ belongs both segments, but occurs twice in subsegment $4 \ldots 5$).</p><p>Help the Fair Nut to find out the number of pairs of good subsegments! The answer can be rather big so print it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— the array elements.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the number of pairs of good subsegments modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— the array elements.</p>

## Output

<p>Print single integer&nbsp;— the number of pairs of good subsegments modulo $10^9+7$.</p>





```input1
3
1 2 3

```




```input2
5
1 2 1 2 3

```




```output1
1

```




```output2
4

```



## Note

<p>In the first example, there is only one pair of good subsegments: $(1 \ldots 2, 2 \ldots 3)$.</p><p>In the second example, there are four pairs of good subsegments: </p><ul> <li> $(1 \ldots 2, 2 \ldots 3)$ </li><li> $(2 \ldots 3, 3 \ldots 4)$ </li><li> $(2 \ldots 3, 3 \ldots 5)$ </li><li> $(3 \ldots 4, 4 \ldots 5)$ </li></ul>
