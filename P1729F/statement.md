## Description

<div><p>Given the string $s$ of decimal digits (<span class="tex-font-style-tt">0</span>-<span class="tex-font-style-tt">9</span>) of length $n$.</p><p>A substring is a sequence of consecutive characters of a string. The substring of this string is defined by a pair of indexes — with its left and right ends. So, each pair of indexes ($l, r$), where $1 \le l \le r \le n$, corresponds to a substring of the string $s$. We will define as $v(l,r)$ the numeric value of the corresponding substring (leading zeros are allowed in it).</p><p>For example, if $n=7$, $s=$"<span class="tex-font-style-tt">1003004</span>", then $v(1,3)=100$, $v(2,3)=0$ and $v(2,7)=3004$.</p><p>You are given $n$, $s$ and an integer $w$ ($1 \le w &lt; n$).</p><p>You need to process $m$ queries, each of which is characterized by $3$ numbers $l_i, r_i, k_i$ ($1 \le l_i \le r_i \le n; 0 \le k_i \le 8$).</p><p>The answer to the $i$th query is such a pair of substrings of length $w$ that if we denote them as $(L_1, L_1+w-1)$ and $(L_2, L_2+w-1)$, then:</p><ul> <li> $L_1 \ne L_2$, that is, the substrings are different; </li><li> the remainder of dividing a number $v(L_1, L_1+w-1) \cdot v(l_i, r_i) + v(L_2, L_2 + w - 1)$ by $9$ is equal to $k_i$. </li></ul><p>If there are many matching substring pairs, then find a pair where $L_1$ is as small as possible. If there are many matching pairs in this case, then minimize $L_2$.</p><p>Note that the answer may not exist.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— number of input test cases.</p><p>The first line of each test case contains a string $s$, which contains only the characters <span class="tex-font-style-tt">0</span>-<span class="tex-font-style-tt">9</span> and has a length $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line contains two integers $w, m$ ($1 \le w &lt; n, 1 \le m \le 2 \cdot 10^5$), where $n$ — is the length of the given string $s$. The number $w$ denotes the lengths of the substrings being searched for, and $m$ is the number of queries to be processed.</p><p>The following $m$ lines contain integers $l_i, r_i, k_i$ ($1 \le l_i \le r_i \le n$, $0 \le k_i \le 8$)&nbsp;— $i$th query parameters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. It is also guaranteed that the sum of $m$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each request, print in a separate line: </p><ul> <li> left borders of the required substrings: $L_1$ and $L_2$; </li><li><span class="tex-font-style-tt">-1 -1</span> otherwise, if there is no solution. </li></ul><p>If there are several solutions, minimize $L_1$ first, and minimize $L_2$ second.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— number of input test cases.</p><p>The first line of each test case contains a string $s$, which contains only the characters <span class="tex-font-style-tt">0</span>-<span class="tex-font-style-tt">9</span> and has a length $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line contains two integers $w, m$ ($1 \le w &lt; n, 1 \le m \le 2 \cdot 10^5$), where $n$ — is the length of the given string $s$. The number $w$ denotes the lengths of the substrings being searched for, and $m$ is the number of queries to be processed.</p><p>The following $m$ lines contain integers $l_i, r_i, k_i$ ($1 \le l_i \le r_i \le n$, $0 \le k_i \le 8$)&nbsp;— $i$th query parameters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. It is also guaranteed that the sum of $m$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each request, print in a separate line: </p><ul> <li> left borders of the required substrings: $L_1$ and $L_2$; </li><li><span class="tex-font-style-tt">-1 -1</span> otherwise, if there is no solution. </li></ul><p>If there are several solutions, minimize $L_1$ first, and minimize $L_2$ second.</p>





```input1|2,3,4,9,10,11,16,17,18,19,20,21,22
5
1003004
4 1
1 2 1
179572007
4 2
2 7 3
2 7 4
111
2 1
2 2 6
0000
1 2
1 4 0
1 4 1
484
1 5
2 2 0
2 3 7
1 2 5
3 3 8
2 2 6
```




```output1
2 4
1 5
1 2
-1 -1
1 2
-1 -1
1 3
1 3
-1 -1
-1 -1
-1 -1
```



## Note

<p>Consider the first test case of example inputs. In this test case $n=7$, $s=$"<span class="tex-font-style-tt">1003004</span>", $w=4$ and one query $l_1=1$, $r_1=2$, $k_1=1$. Note that $v(1,2)=10$. We need to find a pair of substrings of length $4$ such that $v(L_1, L_1+3)\cdot10+v(L_2,L_2+3)$ has a remainder of $k_1=1$ when divided by $9$. The values $L_1=2, L_2=4$ actually satisfy all the requirements: $v(L_1, L_1+w-1)=v(2,5)=30$, $v(L_2, L_2+w-1)=v(4,7)=3004$. Indeed, $30\cdot10+3004=3304$, which has a remainder of $1$ when divided by $9$. It can be shown that $L_1=2$ is the minimum possible value, and $L_2=4$ is the minimum possible with $L_1=2$.</p>
