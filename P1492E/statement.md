## Description

<div><p>You are storing an integer array of length $m$ in a database. To maintain internal integrity and protect data, the database stores $n$ copies of this array.</p><p>Unfortunately, the recent incident may have altered the stored information in every copy in the database.</p><p>It's believed, that the incident altered at most two elements in every copy. You need to recover the original array based on the current state of the database.</p><p>In case there are multiple ways to restore the array, report any. If there is no array that differs from every copy in no more than two positions, report that as well.</p></div><div class="input-specification"><p>The first line contains integers $n$ and $m$ ($2 \le n$; $1 \le m$; $n \cdot m \le 250\,000$)&nbsp;— the number of copies and the size of the array.</p><p>Each of the following $n$ lines describes one of the currently stored copies in the database, it consists of $m$ integers $s_{i, 1}, s_{i, 2}, \dots, s_{i, m}$ ($1 \le s_{i, j} \le 10^9$).</p></div><div class="output-specification"><p>If there is an array consistent with all given copies, print "<span class="tex-font-style-tt">Yes</span>" and then the array itself. The array must have length $m$ and contain integers between $1$ and $10^9$ only.</p><p>Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>If there are multiple possible arrays, print any of them.</p></div>

## Input

<p>The first line contains integers $n$ and $m$ ($2 \le n$; $1 \le m$; $n \cdot m \le 250\,000$)&nbsp;— the number of copies and the size of the array.</p><p>Each of the following $n$ lines describes one of the currently stored copies in the database, it consists of $m$ integers $s_{i, 1}, s_{i, 2}, \dots, s_{i, m}$ ($1 \le s_{i, j} \le 10^9$).</p>

## Output

<p>If there is an array consistent with all given copies, print "<span class="tex-font-style-tt">Yes</span>" and then the array itself. The array must have length $m$ and contain integers between $1$ and $10^9$ only.</p><p>Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>If there are multiple possible arrays, print any of them.</p>





```input1
3 4
1 10 10 100
1 1 1 100
10 100 1 100
```




```input2
10 7
1 1 1 1 1 1 1
1 1 1 1 1 1 2
1 1 1 1 1 2 2
1 1 1 1 2 2 1
1 1 1 2 2 1 1
1 1 2 2 1 1 1
1 2 2 1 1 1 1
2 2 1 1 1 1 1
2 1 1 1 1 1 1
1 1 1 1 1 1 1
```




```input3
2 5
2 2 1 1 1
1 1 2 2 2
```




```output1
Yes
1 10 1 100
```




```output2
Yes
1 1 1 1 1 1 1
```




```output3
No
```



## Note

<p>In the first example, the array $[1, 10, 1, 100]$ differs from first and second copies in just one position, and from the third copy in two positions.</p><p>In the second example, array $[1, 1, 1, 1, 1, 1, 1]$ is the same as the first copy and differs from all other copies in at most two positions.</p><p>In the third example, there is no array differing in at most two positions from every database's copy.</p>
