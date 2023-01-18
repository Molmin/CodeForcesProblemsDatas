## Description

<div><p>You are given an array $a$ consisting of $n$ integers.</p><p>You can remove <span class="tex-font-style-bf">at most one</span> element from this array. Thus, the final length of the array is $n-1$ or $n$.</p><p>Your task is to calculate the maximum possible length of the <span class="tex-font-style-bf">strictly increasing</span> contiguous subarray of the remaining array.</p><p>Recall that the contiguous subarray $a$ with indices from $l$ to $r$ is $a[l \dots r] = a_l, a_{l + 1}, \dots, a_r$. The subarray $a[l \dots r]$ is called strictly increasing if $a_l &lt; a_{l+1} &lt; \dots &lt; a_r$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the $i$-th element of $a$.</p></div><div class="output-specification"><p>Print one integer — the maximum possible length of the <span class="tex-font-style-bf">strictly increasing</span> contiguous subarray of the array $a$ after removing at most one element.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the $i$-th element of $a$.</p>

## Output

<p>Print one integer — the maximum possible length of the <span class="tex-font-style-bf">strictly increasing</span> contiguous subarray of the array $a$ after removing at most one element.</p>





```input1
5
1 2 5 3 4
```




```input2
2
1 2
```




```input3
7
6 5 4 3 2 4 3
```




```output1
4
```




```output2
2
```




```output3
2
```



## Note

<p>In the first example, you can delete $a_3=5$. Then the resulting array will be equal to $[1, 2, 3, 4]$ and the length of its largest increasing subarray will be equal to $4$.</p>
