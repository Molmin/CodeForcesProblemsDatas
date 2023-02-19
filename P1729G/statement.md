## Description

<div><p>You are given two non-empty strings $s$ and $t$, consisting of Latin letters.</p><p>In one move, you can choose an occurrence of the string $t$ in the string $s$ and replace it with dots.</p><p>Your task is to remove all occurrences of the string $t$ in the string $s$ in the minimum number of moves, and also calculate how many <span class="tex-font-style-bf">different</span> sequences of moves of the minimum length exist.</p><p>Two sequences of moves are considered different if the sets of indices at which the removed occurrences of the string $t$ in $s$ begin differ. For example, the sets $\{1, 2, 3\}$ and $\{1, 2, 4\}$ are considered different, the sets $\{2, 4, 6\}$ and $\{2, 6\}$ — too, but sets $\{3, 5\}$ and $\{5, 3\}$ — not.</p><p>For example, let the string $s =$ "<span class="tex-font-style-tt">abababacababa</span>" and the string $t =$ "<span class="tex-font-style-tt">aba</span>". We can remove all occurrences of the string $t$ in $2$ moves by cutting out the occurrences of the string $t$ at the $3$th and $9$th positions. In this case, the string $s$ is an example of the form "<span class="tex-font-style-tt">ab...bac...ba</span>". It is also possible to cut occurrences of the string $t$ at the $3$th and $11$th positions. There are two different sequences of minimum length moves.</p><p>Since the answer can be large, output it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $q$ ($1 \le q \le 50$)&nbsp;— the number of test cases. The descriptions of the sets follow.</p><p>The first line of each set contains a non-empty string $s$ ($1 \le |s| \le 500$) consisting of lowercase Latin letters.</p><p>The second line of each set contains a non-empty string $t$ ($1 \le |t| \le 500$) consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of string lengths $s$ over all test cases does not exceed $500$. Similarly, it is guaranteed that the sum of string lengths $t$ over all test cases does not exceed $500$.</p></div><div class="output-specification"><p>For each test case print two integers — the minimum number of moves and the number of different optimal sequences, modulo $10^9 + 7$.</p></div>

## Input

<p>The first line of the input contains a single integer $q$ ($1 \le q \le 50$)&nbsp;— the number of test cases. The descriptions of the sets follow.</p><p>The first line of each set contains a non-empty string $s$ ($1 \le |s| \le 500$) consisting of lowercase Latin letters.</p><p>The second line of each set contains a non-empty string $t$ ($1 \le |t| \le 500$) consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of string lengths $s$ over all test cases does not exceed $500$. Similarly, it is guaranteed that the sum of string lengths $t$ over all test cases does not exceed $500$.</p>

## Output

<p>For each test case print two integers — the minimum number of moves and the number of different optimal sequences, modulo $10^9 + 7$.</p>





```input1|2,3,6,7,10,11,14,15
8
abababacababa
aba
ddddddd
dddd
xyzxyz
xyz
abc
abcd
abacaba
abaca
abc
def
aaaaaaaa
a
aaaaaaaa
aa
```




```output1
2 2
1 4
2 1
0 1
1 1
0 1
8 1
3 6
```



## Note

<p>The first test case is explained in the statement.</p><p>In the second case, it is enough to cut any of the four occurrences.</p><p>In the third case, string $s$ is the concatenation of two strings $t =$ "<span class="tex-font-style-tt">xyz</span>", so there is a unique optimal sequence of $2$ moves.</p><p>In the fourth and sixth cases, the string $s$ initially contains no occurrences of the string $t$.</p><p>In the fifth case, the string $s$ contains exactly one occurrence of the string $t$.</p>
