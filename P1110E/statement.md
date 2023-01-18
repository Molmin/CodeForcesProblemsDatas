## Description

<div><p>Grigory has $n$ magic stones, conveniently numbered from $1$ to $n$. The <span class="tex-font-style-it">charge</span> of the $i$-th stone is equal to $c_i$.</p><p>Sometimes Grigory gets bored and selects some <span class="tex-font-style-it">inner</span> stone (that is, some stone with index $i$, where $2 \le i \le n - 1$), and after that <span class="tex-font-style-it">synchronizes</span> it with neighboring stones. After that, the chosen stone loses its own charge, but acquires the charges from neighboring stones. In other words, its charge $c_i$ changes to $c_i' = c_{i + 1} + c_{i - 1} - c_i$.</p><p>Andrew, Grigory's friend, also has $n$ stones with charges $t_i$. Grigory is curious, whether there exists a sequence of zero or more <span class="tex-font-style-it">synchronization</span> operations, which transforms charges of Grigory's stones into charges of corresponding Andrew's stones, that is, changes $c_i$ into $t_i$ for all $i$?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of magic stones.</p><p>The second line contains integers $c_1, c_2, \ldots, c_n$ ($0 \le c_i \le 2 \cdot 10^9$)&nbsp;— the charges of Grigory's stones.</p><p>The second line contains integers $t_1, t_2, \ldots, t_n$ ($0 \le t_i \le 2 \cdot 10^9$)&nbsp;— the charges of Andrew's stones.</p></div><div class="output-specification"><p>If there exists a (possibly empty) sequence of <span class="tex-font-style-it">synchronization</span> operations, which changes all charges to the required ones, print "<span class="tex-font-style-tt">Yes</span>".</p><p>Otherwise, print "<span class="tex-font-style-tt">No</span>".</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of magic stones.</p><p>The second line contains integers $c_1, c_2, \ldots, c_n$ ($0 \le c_i \le 2 \cdot 10^9$)&nbsp;— the charges of Grigory's stones.</p><p>The second line contains integers $t_1, t_2, \ldots, t_n$ ($0 \le t_i \le 2 \cdot 10^9$)&nbsp;— the charges of Andrew's stones.</p>

## Output

<p>If there exists a (possibly empty) sequence of <span class="tex-font-style-it">synchronization</span> operations, which changes all charges to the required ones, print "<span class="tex-font-style-tt">Yes</span>".</p><p>Otherwise, print "<span class="tex-font-style-tt">No</span>".</p>





```input1
4
7 2 4 12
7 15 10 12
```




```input2
3
4 4 4
1 2 3
```




```output1
Yes
```




```output2
No
```



## Note

<p>In the first example, we can perform the following <span class="tex-font-style-it">synchronizations</span> ($1$-indexed):</p><ul> <li> First, <span class="tex-font-style-it">synchronize</span> the third stone $[7, 2, \mathbf{4}, 12] \rightarrow [7, 2, \mathbf{10}, 12]$. </li><li> Then <span class="tex-font-style-it">synchronize</span> the second stone: $[7, \mathbf{2}, 10, 12] \rightarrow [7, \mathbf{15}, 10, 12]$. </li></ul><p>In the second example, any operation with the second stone will not change its charge.</p>
