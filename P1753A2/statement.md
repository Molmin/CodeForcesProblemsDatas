## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference is that in this version the array contains zeros. You can make hacks only if both versions of the problem are solved.</span></p><p>You are given an array $[a_1, a_2, \ldots a_n]$ consisting of integers $-1$, $0$ and $1$. You have to build a partition of this array into the set of segments $[l_1, r_1], [l_2, r_2], \ldots, [l_k, r_k]$ with the following property:</p><ul> <li> Denote the alternating sum of all elements of the $i$-th segment as $s_i$: $s_i$ = $a_{l_i} - a_{l_i+1} + a_{l_i+2} - a_{l_i+3} + \ldots \pm a_{r_i}$. For example, the alternating sum of elements of segment $[2, 4]$ in array $[1, 0, -1, 1, 1]$ equals to $0 - (-1) + 1 = 2$. </li><li> The sum of $s_i$ over all segments of partition should be equal to zero. </li></ul><p>Note that each $s_i$ does <span class="tex-font-style-bf">not</span> have to be equal to zero, this property is about sum of $s_i$ over all segments of partition.</p><p>The set of segments $[l_1, r_1], [l_2, r_2], \ldots, [l_k, r_k]$ is called a <span class="tex-font-style-bf">partition</span> of the array $a$ of length $n$ if $1 = l_1 \le r_1, l_2 \le r_2, \ldots, l_k \le r_k = n$ and $r_i + 1 = l_{i+1}$ for all $i = 1, 2, \ldots k-1$. In other words, each element of the array must belong to exactly one segment.</p><p>You have to build a partition of the given array with properties described above or determine that such partition does not exist.</p><p>Note that it is <span class="tex-font-style-bf">not</span> required to minimize the number of segments in the partition.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 200\,000$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($a_i$ is $-1$, $0$, or $1$)&nbsp;— the elements of the given array.</p><p>It's guaranteed that the sum of $n$ over all test cases does not exceed $200\,000$.</p></div><div class="output-specification"><p>For each test case print an integer $k$&nbsp;— the number of segments in the partition. If required partition does not exist, print $-1$.</p><p>If partition exists, in the $i$-th of the following $k$ lines print two integers $l_i$ and $r_i$&nbsp;— description of the $i$-th segment. The following conditions should be satisfied:</p><ul> <li> $l_i \le r_i$ for each $i$ from $1$ to $k$. </li><li> $l_{i + 1} = r_i + 1$ for each $i$ from $1$ to $(k - 1)$. </li><li> $l_1 = 1, r_k = n$. </li></ul><p>If there are multiple correct partitions of the array, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 200\,000$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($a_i$ is $-1$, $0$, or $1$)&nbsp;— the elements of the given array.</p><p>It's guaranteed that the sum of $n$ over all test cases does not exceed $200\,000$.</p>

## Output

<p>For each test case print an integer $k$&nbsp;— the number of segments in the partition. If required partition does not exist, print $-1$.</p><p>If partition exists, in the $i$-th of the following $k$ lines print two integers $l_i$ and $r_i$&nbsp;— description of the $i$-th segment. The following conditions should be satisfied:</p><ul> <li> $l_i \le r_i$ for each $i$ from $1$ to $k$. </li><li> $l_{i + 1} = r_i + 1$ for each $i$ from $1$ to $(k - 1)$. </li><li> $l_1 = 1, r_k = n$. </li></ul><p>If there are multiple correct partitions of the array, print any of them.</p>





```input1|2,3,6,7,10,11
5
4
0 0 0 0
7
-1 1 0 1 0 1 0
5
0 -1 1 0 1
3
1 0 1
1
1
```




```output1
4
1 1
2 2
3 3
4 4
4
1 1
2 2
3 5
6 7
-1
2
1 1
2 3
-1
```



## Note

<p>In the first test case we can build a partition of $4$ segments&nbsp;— each of them will contain only one element of the array equals to $0$. So the sum will be equal to $0 + 0 + 0 + 0 = 0$.</p><p>In the second test case we can build a partition of $4$ segments. The alternating sum of the first segment will be equal to $-1$, the alternating sum of the second segment will be equal to $1$, of the third segment&nbsp;— $0 - 1 + 0 = -1$, of the fourth segment&nbsp;— $1 - 0 = 1$. The sum will be equal to $-1 + 1 -1 + 1 = 0$.</p><p>In the third test case it can be proved that the required partition does not exist.</p>
