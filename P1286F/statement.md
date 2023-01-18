## Description

<div><p>To defeat Lord Voldemort, Harry needs to destroy all horcruxes first. The last horcrux is an array $a$ of $n$ integers, which also needs to be destroyed. The array is considered destroyed if all its elements are zeroes. To destroy the array, Harry can perform two types of operations:</p><ol> <li> choose an index $i$ ($1 \le i \le n$), an integer $x$, and subtract $x$ from $a_i$.</li><li> choose two indices $i$ and $j$ ($1 \le i, j \le n; i \ne j$), an integer $x$, and subtract $x$ from $a_i$ and $x + 1$ from $a_j$. </li></ol><p>Note that $x$ does not have to be positive.</p><center><img class="tex-graphics" src="file://uKzIahgt.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Harry is in a hurry, please help him to find the minimum number of operations required to destroy the array and exterminate Lord Voldemort.</p></div><div class="input-specification"><p>The first line contains a single integer $n$&nbsp;— the size of the array $a$ ($1 \le n \le 20$). </p><p>The following line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— array elements ($-10^{15} \le a_i \le 10^{15}$).</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the minimum number of operations required to destroy the array $a$.</p></div>

## Input

<p>The first line contains a single integer $n$&nbsp;— the size of the array $a$ ($1 \le n \le 20$). </p><p>The following line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— array elements ($-10^{15} \le a_i \le 10^{15}$).</p>

## Output

<p>Output a single integer&nbsp;— the minimum number of operations required to destroy the array $a$.</p>





```input1
3
1 10 100
```




```input2
3
5 3 -2
```




```input3
1
0
```




```output1
3
```




```output2
2
```




```output3
0
```



## Note

<p>In the first example one can just apply the operation of the first kind three times.</p><p>In the second example, one can apply the operation of the second kind two times: first, choose $i = 2, j = 1, x = 4$, it transforms the array into $(0, -1, -2)$, and then choose $i = 3, j = 2, x = -2$ to destroy the array.</p><p>In the third example, there is nothing to be done, since the array is already destroyed.</p>
