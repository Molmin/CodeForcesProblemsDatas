## Description

<div><p>An array $b$ is called to be a <span class="tex-font-style-it">subarray</span> of $a$ if it forms a continuous subsequence of $a$, that is, if it is equal to $a_l$, $a_{l + 1}$, $\ldots$, $a_r$ for some $l, r$.</p><p>Suppose $m$ is some known constant. For any array, having $m$ or more elements, let's define it's <span class="tex-font-style-it">beauty</span> as the sum of $m$ largest elements of that array. For example: </p><ul> <li> For array $x = [4, 3, 1, 5, 2]$ and $m = 3$, the $3$ largest elements of $x$ are $5$, $4$ and $3$, so the beauty of $x$ is $5 + 4 + 3 = 12$.</li><li> For array $x = [10, 10, 10]$ and $m = 2$, the beauty of $x$ is $10 + 10 = 20$.</li></ul><p>You are given an array $a_1, a_2, \ldots, a_n$, the value of the said constant $m$ and an integer $k$. Your need to split the array $a$ into exactly $k$ subarrays such that:</p><ul> <li> Each element from $a$ belongs to exactly one subarray.</li><li> Each subarray has at least $m$ elements.</li><li> The sum of all beauties of $k$ subarrays is maximum possible.</li></ul></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $k$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m$, $2 \le k$, $m \cdot k \le n$)&nbsp;— the number of elements in $a$, the constant $m$ in the definition of beauty and the number of subarrays to split to.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>In the first line, print the maximum possible sum of the beauties of the subarrays in the optimal partition.</p><p>In the second line, print $k-1$ integers $p_1, p_2, \ldots, p_{k-1}$ ($1 \le p_1 &lt; p_2 &lt; \ldots &lt; p_{k-1} &lt; n$) representing the partition of the array, in which:</p><ul><li> All elements with indices from $1$ to $p_1$ belong to the first subarray.</li><li> All elements with indices from $p_1 + 1$ to $p_2$ belong to the second subarray.</li><li> $\ldots$.</li><li> All elements with indices from $p_{k-1} + 1$ to $n$ belong to the last, $k$-th subarray.</li></ul><p>If there are several optimal partitions, print any of them.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $k$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m$, $2 \le k$, $m \cdot k \le n$)&nbsp;— the number of elements in $a$, the constant $m$ in the definition of beauty and the number of subarrays to split to.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$).</p>

## Output

<p>In the first line, print the maximum possible sum of the beauties of the subarrays in the optimal partition.</p><p>In the second line, print $k-1$ integers $p_1, p_2, \ldots, p_{k-1}$ ($1 \le p_1 &lt; p_2 &lt; \ldots &lt; p_{k-1} &lt; n$) representing the partition of the array, in which:</p><ul><li> All elements with indices from $1$ to $p_1$ belong to the first subarray.</li><li> All elements with indices from $p_1 + 1$ to $p_2$ belong to the second subarray.</li><li> $\ldots$.</li><li> All elements with indices from $p_{k-1} + 1$ to $n$ belong to the last, $k$-th subarray.</li></ul><p>If there are several optimal partitions, print any of them.</p>





```input1
9 2 3
5 2 5 2 4 1 1 3 2
```




```input2
6 1 4
4 1 3 2 2 3
```




```input3
2 1 2
-1000000000 1000000000
```




```output1
21
3 5
```




```output2
12
1 3 5
```




```output3
0
1
```



## Note

<p>In the first example, one of the optimal partitions is $[5, 2, 5]$, $[2, 4]$, $[1, 1, 3, 2]$.</p><ul> <li> The beauty of the subarray $[5, 2, 5]$ is $5 + 5 = 10$. </li><li> The beauty of the subarray $[2, 4]$ is $2 + 4 = 6$. </li><li> The beauty of the subarray $[1, 1, 3, 2]$ is $3 + 2 = 5$. </li></ul><p>The sum of their beauties is $10 + 6 + 5 = 21$.</p><p>In the second example, one optimal partition is $[4]$, $[1, 3]$, $[2, 2]$, $[3]$.</p>
