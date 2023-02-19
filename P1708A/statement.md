## Description

<div><p>You are given an array $a$ consisting of $n$ positive integers.</p><p>You are allowed to perform this operation any number of times (possibly, zero): </p><ul> <li> choose an index $i$ ($2 \le i \le n$), and change $a_i$ to $a_i - a_{i-1}$. </li></ul><p>Is it possible to make $a_i=0$ for all $2\le i\le n$?</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 100$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line contains one integer $n$ ($2 \le n \le 100$)&nbsp;— the length of array $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes), if it is possible to change $a_i$ to $0$ for all $2 \le i \le n$, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can print letters in any case (upper or lower).</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 100$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line contains one integer $n$ ($2 \le n \le 100$)&nbsp;— the length of array $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le 10^9$).</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes), if it is possible to change $a_i$ to $0$ for all $2 \le i \le n$, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can print letters in any case (upper or lower).</p>





```input1|2,3,6,7
4
2
5 10
3
1 2 3
4
1 1 1 1
9
9 9 8 2 4 4 3 5 3
```




```output1
YES
YES
YES
NO
```



## Note

<p>In the first test case, the initial array is $[5,10]$. You can perform $2$ operations to reach the goal:</p><ol> <li> Choose $i=2$, and the array becomes $[5,5]$. </li><li> Choose $i=2$, and the array becomes $[5,0]$. </li></ol><p>In the second test case, the initial array is $[1,2,3]$. You can perform $4$ operations to reach the goal: </p><ol> <li> Choose $i=3$, and the array becomes $[1,2,1]$. </li><li> Choose $i=2$, and the array becomes $[1,1,1]$. </li><li> Choose $i=3$, and the array becomes $[1,1,0]$. </li><li> Choose $i=2$, and the array becomes $[1,0,0]$. </li></ol><p>In the third test case, you can choose indices in the order $4$, $3$, $2$.</p>
