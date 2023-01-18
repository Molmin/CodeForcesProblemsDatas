## Description

<div><p>You are given an array $a_1, a_2, \ldots, a_n$.</p><p>In one operation you can choose two elements $a_i$ and $a_j$ ($i \ne j$) and decrease each of them by one.</p><p>You need to check whether it is possible to make all the elements equal to zero or not.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the size of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if it is possible to make all elements zero, otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the size of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if it is possible to make all elements zero, otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
4
1 1 2 2
```




```input2
6
1 2 3 4 5 6
```




```output1
YES
```




```output2
NO
```



## Note

<p>In the first example, you can make all elements equal to zero in $3$ operations: </p><ul> <li> Decrease $a_1$ and $a_2$, </li><li> Decrease $a_3$ and $a_4$, </li><li> Decrease $a_3$ and $a_4$ </li></ul><p>In the second example, one can show that it is impossible to make all elements equal to zero.</p>
