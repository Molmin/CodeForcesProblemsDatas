## Description

<div><p>To satisfy his love of matching socks, Phoenix has brought his $n$ socks ($n$ is even) to the sock store. Each of his socks has a color $c_i$ and is either a left sock or right sock. </p><p>Phoenix can pay one dollar to the sock store to either: </p><ul> <li> recolor a sock to any color $c'$ $(1 \le c' \le n)$ </li><li> turn a left sock into a right sock </li><li> turn a right sock into a left sock </li></ul> <p>The sock store may perform each of these changes any number of times. Note that the color of a left sock doesn't change when it turns into a right sock, and vice versa. </p><p>A matching pair of socks is a left and right sock with the same color. What is the minimum cost for Phoenix to make $n/2$ matching pairs? Each sock must be included in exactly one matching pair.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains three integers $n$, $l$, and $r$ ($2 \le n \le 2 \cdot 10^5$; $n$ is even; $0 \le l, r \le n$; $l+r=n$)&nbsp;— the total number of socks, and the number of left and right socks, respectively.</p><p>The next line contains $n$ integers $c_i$ ($1 \le c_i \le n$)&nbsp;— the colors of the socks. The first $l$ socks are left socks, while the next $r$ socks are right socks.</p><p>It is guaranteed that the sum of $n$ across all the test cases will not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the minimum cost for Phoenix to make $n/2$ matching pairs. Each sock must be included in exactly one matching pair.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains three integers $n$, $l$, and $r$ ($2 \le n \le 2 \cdot 10^5$; $n$ is even; $0 \le l, r \le n$; $l+r=n$)&nbsp;— the total number of socks, and the number of left and right socks, respectively.</p><p>The next line contains $n$ integers $c_i$ ($1 \le c_i \le n$)&nbsp;— the colors of the socks. The first $l$ socks are left socks, while the next $r$ socks are right socks.</p><p>It is guaranteed that the sum of $n$ across all the test cases will not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer&nbsp;— the minimum cost for Phoenix to make $n/2$ matching pairs. Each sock must be included in exactly one matching pair.</p>





```input1
4
6 3 3
1 2 3 2 2 2
6 2 4
1 1 2 2 2 2
6 5 1
6 5 4 3 2 1
4 0 4
4 4 4 3
```




```output1
2
3
5
3
```



## Note

<p>In the first test case, Phoenix can pay $2$ dollars to: </p><ul> <li> recolor sock $1$ to color $2$ </li><li> recolor sock $3$ to color $2$ </li></ul> There are now $3$ matching pairs. For example, pairs $(1, 4)$, $(2, 5)$, and $(3, 6)$ are matching.<p>In the second test case, Phoenix can pay $3$ dollars to: </p><ul> <li> turn sock $6$ from a right sock to a left sock </li><li> recolor sock $3$ to color $1$ </li><li> recolor sock $4$ to color $1$ </li></ul> There are now $3$ matching pairs. For example, pairs $(1, 3)$, $(2, 4)$, and $(5, 6)$ are matching.
