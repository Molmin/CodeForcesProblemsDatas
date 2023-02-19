## Description

<div><p>You have two strings $a$ and $b$ of equal length $n$ consisting of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>, and an integer $k$.</p><p>You need to make strings $a$ and $b$ equal.</p><p>In one step, you can choose any substring of $a$ containing exactly $k$ characters <span class="tex-font-style-tt">1</span> (and arbitrary number of characters <span class="tex-font-style-tt">0</span>) and reverse it. Formally, if $a = a_1 a_2 \ldots a_n$, you can choose any integers $l$ and $r$ ($1 \le l \le r \le n$) such that there are exactly $k$ ones among characters $a_l, a_{l+1}, \ldots, a_r$, and set $a$ to $a_1 a_2 \ldots a_{l-1} a_r a_{r-1} \ldots a_l a_{r+1} a_{r+2} \ldots a_n$.</p><p>Find a way to make $a$ equal to $b$ using at most $4n$ reversals of the above kind, or determine that such a way doesn't exist. The number of reversals doesn't have to be minimized.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2000$). Description of the test cases follows.</p><p>Each test case consists of three lines. The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2000$; $0 \le k \le n$).</p><p>The second line contains string $a$ of length $n$.</p><p>The third line contains string $b$ of the same length. Both strings consist of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, if it's impossible to make $a$ equal to $b$ in at most $4n$ reversals, print a single integer $-1$.</p><p>Otherwise, print an integer $m$ ($0 \le m \le 4n$), denoting the number of reversals in your sequence of steps, followed by $m$ pairs of integers $l_i, r_i$ ($1 \le l_i \le r_i \le n$), denoting the boundaries of the substrings of $a$ to be reversed, in chronological order. Each substring must contain exactly $k$ ones at the moment of reversal.</p><p>Note that $m$ doesn't have to be minimized. If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2000$). Description of the test cases follows.</p><p>Each test case consists of three lines. The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2000$; $0 \le k \le n$).</p><p>The second line contains string $a$ of length $n$.</p><p>The third line contains string $b$ of the same length. Both strings consist of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, if it's impossible to make $a$ equal to $b$ in at most $4n$ reversals, print a single integer $-1$.</p><p>Otherwise, print an integer $m$ ($0 \le m \le 4n$), denoting the number of reversals in your sequence of steps, followed by $m$ pairs of integers $l_i, r_i$ ($1 \le l_i \le r_i \le n$), denoting the boundaries of the substrings of $a$ to be reversed, in chronological order. Each substring must contain exactly $k$ ones at the moment of reversal.</p><p>Note that $m$ doesn't have to be minimized. If there are multiple answers, print any.</p>





```input1
6
6 1
101010
010101
6 3
101010
010101
6 0
101010
010101
6 6
101010
010101
4 2
0000
1111
9 2
011100101
101001011
```




```output1
3
1 2
3 4
5 6
1
1 6
-1
-1
-1
5
4 8
8 9
3 6
1 4
3 6
```



## Note

<p>In the first test case, after the first reversal $a = $ <span class="tex-font-style-tt">011010</span>, after the second reversal $a = $ <span class="tex-font-style-tt">010110</span>, after the third reversal $a = $ <span class="tex-font-style-tt">010101</span>.</p>
