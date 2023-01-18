## Description

<div><p>You are given an array $a_{1}, a_{2}, \ldots, a_{n}$. You can remove <span class="tex-font-style-bf">at most one</span> subsegment from it. The remaining elements should be pairwise distinct.</p><p>In other words, <span class="tex-font-style-bf">at most one</span> time you can choose two integers $l$ and $r$ ($1 \leq l \leq r \leq n$) and delete integers $a_l, a_{l+1}, \ldots, a_r$ from the array. Remaining elements should be pairwise distinct. </p><p>Find the minimum size of the subsegment you need to remove to make all remaining elements distinct.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($1 \le n \le 2000$)&nbsp;— the number of elements in the given array.</p><p>The next line contains $n$ spaced integers $a_{1}, a_{2}, \ldots, a_{n}$ ($1 \le a_{i} \le 10^{9}$)&nbsp;— the elements of the array. </p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum size of the subsegment you need to remove to make all elements of the array pairwise distinct. If no subsegment needs to be removed, print $0$.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($1 \le n \le 2000$)&nbsp;— the number of elements in the given array.</p><p>The next line contains $n$ spaced integers $a_{1}, a_{2}, \ldots, a_{n}$ ($1 \le a_{i} \le 10^{9}$)&nbsp;— the elements of the array. </p>

## Output

<p>Print a single integer&nbsp;— the minimum size of the subsegment you need to remove to make all elements of the array pairwise distinct. If no subsegment needs to be removed, print $0$.</p>





```input1
3
1 2 3
```




```input2
4
1 1 2 2
```




```input3
5
1 4 1 4 9
```




```output1
0
```




```output2
2
```




```output3
2
```



## Note

<p>In the first example all the elements are already distinct, therefore no subsegment needs to be removed.</p><p>In the second example you can remove the subsegment from index $2$ to $3$.</p><p>In the third example you can remove the subsegments from index $1$ to $2$, or from index $2$ to $3$, or from index $3$ to $4$.</p>
