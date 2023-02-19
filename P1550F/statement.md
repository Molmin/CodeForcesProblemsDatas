## Description

<div><p>There is an infinite pond that can be represented with a number line. There are $n$ rocks in the pond, numbered from $1$ to $n$. The $i$-th rock is located at an integer coordinate $a_i$. The coordinates of the rocks are pairwise distinct. The rocks are numbered in the increasing order of the coordinate, so $a_1 &lt; a_2 &lt; \dots &lt; a_n$.</p><p>A robot frog sits on the rock number $s$. The frog is programmable. It has a base jumping distance parameter $d$. There also is a setting for the jumping distance range. If the jumping distance range is set to some integer $k$, then the frog can jump from some rock to any rock at a distance from $d - k$ to $d + k$ inclusive in any direction. The distance between two rocks is an absolute difference between their coordinates.</p><p>You are assigned a task to implement a feature for the frog. Given two integers $i$ and $k$ determine if the frog can reach a rock number $i$ from a rock number $s$ performing a sequence of jumps with the jumping distance range set to $k$. The sequence can be arbitrarily long or empty.</p><p>You will be given $q$ testcases for that feature, the $j$-th testcase consists of two integers $i$ and $k$. Print "<span class="tex-font-style-tt">Yes</span>" if the $i$-th rock is reachable and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and '<span class="tex-font-style-tt">YES</span>"' will be recognized as a positive answer).</p></div><div class="input-specification"><p>The first line contains four integers $n$, $q$, $s$ and $d$ ($1 \le n, q \le 2 \cdot 10^5$; $1 \le s \le n$; $1 \le d \le 10^6$)&nbsp;— the number of rocks, the number of testcases, the starting rock and the base jumping distance parameter.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$)&nbsp;— the coordinates of the rocks. The coordinates of the rocks are pairwise distinct. The rocks are numbered in the increasing order of distance from the land, so $a_1 &lt; a_2 &lt; \dots &lt; a_n$.</p><p>Each of the next $q$ lines contains two integers $i$ and $k$ ($1 \le i \le n$; $1 \le k \le 10^6$)&nbsp;— the parameters to the testcase.</p></div><div class="output-specification"><p>For each of the testcases print an answer. If there is a sequence of jumps from a rock number $s$ to a rock number $i$ with the jumping distance range set to $k$, then print "<span class="tex-font-style-tt">Yes</span>". Otherwise, print "<span class="tex-font-style-tt">No</span>".</p></div>

## Input

<p>The first line contains four integers $n$, $q$, $s$ and $d$ ($1 \le n, q \le 2 \cdot 10^5$; $1 \le s \le n$; $1 \le d \le 10^6$)&nbsp;— the number of rocks, the number of testcases, the starting rock and the base jumping distance parameter.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$)&nbsp;— the coordinates of the rocks. The coordinates of the rocks are pairwise distinct. The rocks are numbered in the increasing order of distance from the land, so $a_1 &lt; a_2 &lt; \dots &lt; a_n$.</p><p>Each of the next $q$ lines contains two integers $i$ and $k$ ($1 \le i \le n$; $1 \le k \le 10^6$)&nbsp;— the parameters to the testcase.</p>

## Output

<p>For each of the testcases print an answer. If there is a sequence of jumps from a rock number $s$ to a rock number $i$ with the jumping distance range set to $k$, then print "<span class="tex-font-style-tt">Yes</span>". Otherwise, print "<span class="tex-font-style-tt">No</span>".</p>





```input1
7 4 4 5
1 5 10 13 20 22 28
4 1
7 2
7 3
3 2
```




```input2
10 8 6 11
1 2 4 7 8 9 11 13 19 20
2 13
5 8
8 1
6 15
1 15
2 7
7 6
8 9
```




```input3
6 9 6 6
1 2 4 9 18 19
2 17
1 18
5 4
2 11
5 17
6 8
4 3
3 3
6 6
```




```input4
4 1 1 10
1 8 10 19
2 1
```




```output1
Yes
No
Yes
Yes
```




```output2
Yes
Yes
No
Yes
Yes
Yes
Yes
Yes
```




```output3
Yes
Yes
Yes
Yes
Yes
Yes
No
No
Yes
```




```output4
Yes
```



## Note

<p>Explanation of the first example:</p><p>In the first testcase the destination rock is the same as the starting rock, thus no jumps are required to reach it.</p><p>In the second testcase the frog can jump any distance in the range $[5 - 2; 5 + 2]$. Thus, it can reach rock number $5$ (by jumping $7$ to the right) and rock number $3$ (by jumping $3$ to the left). From rock number $3$ it can reach rock number $2$ (by jumping $5$ to the left). From rock number $2$ it can reach rock number $1$ (by jumping $4$ to the left). However, there is no way to reach rock number $7$.</p><p>In the third testcase the frog can jump any distance in the range $[5 - 3; 5 + 3]$. Thus, it can reach rock number $7$ by jumping to rock $5$ first and to $7$ afterwards.</p><p>The fourth testcase is shown in the explanation for the second testcase.</p>
