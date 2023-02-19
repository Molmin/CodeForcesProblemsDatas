## Description

<div><p>You are given a string $s$ consisting of the characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>', and '<span class="tex-font-style-tt">?</span>'. You need to replace all the characters with '<span class="tex-font-style-tt">?</span>' in the string $s$ by '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>' so that the string becomes a palindrome and has <span class="tex-font-style-bf">exactly</span> $a$ characters '<span class="tex-font-style-tt">0</span>' and <span class="tex-font-style-bf">exactly</span> $b$ characters '<span class="tex-font-style-tt">1</span>'. Note that each of the characters '<span class="tex-font-style-tt">?</span>' is replaced <span class="tex-font-style-bf">independently</span> from the others.</p><p>A string $t$ of length $n$ is called a palindrome if the equality $t[i] = t[n-i+1]$ is true for all $i$ ($1 \le i \le n$).</p><p>For example, if $s=$"<span class="tex-font-style-tt">01?????0</span>", $a=4$ and $b=4$, then you can replace the characters '<span class="tex-font-style-tt">?</span>' in the following ways: </p><ul> <li> "<span class="tex-font-style-tt">01011010</span>"; </li><li> "<span class="tex-font-style-tt">01100110</span>". </li></ul><p>For the given string $s$ and the numbers $a$ and $b$, replace all the characters with '<span class="tex-font-style-tt">?</span>' in the string $s$ by '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>' so that the string becomes a palindrome and has <span class="tex-font-style-bf">exactly</span> $a$ characters '<span class="tex-font-style-tt">0</span>' and <span class="tex-font-style-bf">exactly</span> $b$ characters '<span class="tex-font-style-tt">1</span>'.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $a$ and $b$ ($0 \le a, b \le 2 \cdot 10^5$, $a + b \ge 1$).</p><p>The second line of each test case contains the string $s$ of length $a+b$, consisting of the characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>', and '<span class="tex-font-style-tt">?</span>'.</p><p>It is guaranteed that the sum of the string lengths of $s$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output: </p><ul> <li> "<span class="tex-font-style-tt">-1</span>", if you can't replace all the characters '<span class="tex-font-style-tt">?</span>' in the string $s$ by '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>' so that the string becomes a palindrome and that it contains <span class="tex-font-style-bf">exactly</span> $a$ characters '<span class="tex-font-style-tt">0</span>' and <span class="tex-font-style-bf">exactly</span> $b$ characters '<span class="tex-font-style-tt">1</span>'; </li><li> the string that is obtained as a result of the replacement, otherwise. </li></ul><p>If there are several suitable ways to replace characters, you can output any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $a$ and $b$ ($0 \le a, b \le 2 \cdot 10^5$, $a + b \ge 1$).</p><p>The second line of each test case contains the string $s$ of length $a+b$, consisting of the characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>', and '<span class="tex-font-style-tt">?</span>'.</p><p>It is guaranteed that the sum of the string lengths of $s$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output: </p><ul> <li> "<span class="tex-font-style-tt">-1</span>", if you can't replace all the characters '<span class="tex-font-style-tt">?</span>' in the string $s$ by '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>' so that the string becomes a palindrome and that it contains <span class="tex-font-style-bf">exactly</span> $a$ characters '<span class="tex-font-style-tt">0</span>' and <span class="tex-font-style-bf">exactly</span> $b$ characters '<span class="tex-font-style-tt">1</span>'; </li><li> the string that is obtained as a result of the replacement, otherwise. </li></ul><p>If there are several suitable ways to replace characters, you can output any.</p>





```input1
9
4 4
01?????0
3 3
??????
1 0
?
2 2
0101
2 2
01?0
0 1
0
0 3
1?1
2 2
?00?
4 3
??010?0
```




```output1
01011010
-1
0
-1
0110
-1
111
1001
0101010
```


