## Description

<div><p>Initially there was an array $a$ consisting of $n$ integers. Positions in it are numbered from $1$ to $n$.</p><p>Exactly $q$ queries were performed on the array. During the $i$-th query some segment $(l_i, r_i)$ $(1 \le l_i \le r_i \le n)$ was selected and values of elements on positions from $l_i$ to $r_i$ inclusive got changed to $i$. The order of the queries couldn't be changed and all $q$ queries were applied. It is also known that every position from $1$ to $n$ got covered by at least one segment.</p><p>We could have offered you the problem about checking if some given array (consisting of $n$ integers with values from $1$ to $q$) can be obtained by the aforementioned queries. However, we decided that it will come too easy for you.</p><p>So the enhancement we introduced to it is the following. Some set of positions (possibly empty) in this array is selected and values of elements on these positions are set to $0$.</p><p>Your task is to check if this array can be obtained by the aforementioned queries. Also if it can be obtained then restore this array.</p><p>If there are multiple possible arrays then print any of them.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$) — the number of elements of the array and the number of queries perfomed on it.</p><p>The second line contains $n$ integer numbers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le q$) — the resulting array. If element at some position $j$ is equal to $0$ then the value of element at this position can be any integer from $1$ to $q$.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if the array $a$ can be obtained by performing $q$ queries. Segments $(l_i, r_i)$ $(1 \le l_i \le r_i \le n)$ are chosen separately for each query. Every position from $1$ to $n$ should be covered by at least one segment. </p><p>Otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>If some array can be obtained then print $n$ integers on the second line — the $i$-th number should be equal to the $i$-th element of the resulting array and should have value from $1$ to $q$. This array should be obtainable by performing exactly $q$ queries.</p><p>If there are multiple possible arrays then print any of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$) — the number of elements of the array and the number of queries perfomed on it.</p><p>The second line contains $n$ integer numbers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le q$) — the resulting array. If element at some position $j$ is equal to $0$ then the value of element at this position can be any integer from $1$ to $q$.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if the array $a$ can be obtained by performing $q$ queries. Segments $(l_i, r_i)$ $(1 \le l_i \le r_i \le n)$ are chosen separately for each query. Every position from $1$ to $n$ should be covered by at least one segment. </p><p>Otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>If some array can be obtained then print $n$ integers on the second line — the $i$-th number should be equal to the $i$-th element of the resulting array and should have value from $1$ to $q$. This array should be obtainable by performing exactly $q$ queries.</p><p>If there are multiple possible arrays then print any of them.</p>





```input1
4 3
1 0 2 3

```




```input2
3 10
10 10 10

```




```input3
5 6
6 5 6 2 2

```




```input4
3 5
0 0 0

```




```output1
YES
1 2 2 3

```




```output2
YES
10 10 10 

```




```output3
NO

```




```output4
YES
5 4 2

```



## Note

<p>In the first example you can also replace $0$ with $1$ but not with $3$.</p><p>In the second example it doesn't really matter what segments to choose until query $10$ when the segment is $(1, 3)$.</p><p>The third example showcases the fact that the order of queries can't be changed, you can't firstly set $(1, 3)$ to $6$ and after that change $(2, 2)$ to $5$. The segment of $5$ should be applied before segment of $6$.</p><p>There is a lot of correct resulting arrays for the fourth example.</p>
