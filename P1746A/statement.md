## Description

<div><p>You have an array $a$ of size $n$ consisting only of zeroes and ones and an integer $k$. In one operation you can do one of the following:</p><ul> <li> Select $2$ consecutive elements of $a$ and replace them with their minimum (that is, let $a := [a_{1}, a_{2}, \ldots, a_{i-1}, \min(a_{i}, a_{i+1}), a_{i+2}, \ldots, a_{n}]$ for some $1 \le i \le n-1$). This operation decreases the size of $a$ by $1$. </li><li> Select $k$ consecutive elements of $a$ and replace them with their maximum (that is, let $a := [a_{1}, a_{2}, \ldots, a_{i-1}, \max(a_{i}, a_{i+1}, \ldots, a_{i+k-1}), a_{i+k}, \ldots, a_{n}]$ for some $1 \le i \le n-k+1$). This operation decreases the size of $a$ by $k-1$. </li></ul><p>Determine if it's possible to turn $a$ into $[1]$ after several (possibly zero) operations.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le k \le n \le 50$), the size of array $a$ and the length of segments that you can perform second type operation on.</p><p>The second line contains $n$ integers $a_{1}, a_{2}, \ldots, a_{n}$ ($a_i$ is $0$ or $1$), elements of array $a$.</p></div><div class="output-specification"><p>For each test case, if it is possible to turn $a$ into $[1]$, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le k \le n \le 50$), the size of array $a$ and the length of segments that you can perform second type operation on.</p><p>The second line contains $n$ integers $a_{1}, a_{2}, \ldots, a_{n}$ ($a_i$ is $0$ or $1$), elements of array $a$.</p>

## Output

<p>For each test case, if it is possible to turn $a$ into $[1]$, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1|2,3,6,7,10,11,14,15
7
3 2
0 1 0
5 3
1 0 1 1 0
2 2
1 1
4 4
0 0 0 0
6 3
0 0 1 0 0 1
7 5
1 1 1 1 1 1 1
5 3
0 0 1 0 0
```




```output1
YES
YES
YES
NO
YES
YES
YES
```



## Note

<p>In the first test case, you can perform the second type operation on second and third elements so $a$ becomes $[0, 1]$, then you can perform the second type operation on first and second elements, so $a$ turns to $[1]$.</p><p>In the fourth test case, it's obvious to see that you can't make any $1$, no matter what you do.</p><p>In the fifth test case, you can first perform a type 2 operation on the first three elements so that $a$ becomes $[1, 0, 0, 1]$, then perform a type 2 operation on the elements in positions two through four, so that $a$ becomes $[1, 1]$, and finally perform the first type operation on the remaining elements, so that $a$ becomes $[1]$.</p>
