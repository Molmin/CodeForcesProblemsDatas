## Description

<div><p>You are given three strings $a$, $b$ and $c$ of the same length $n$. The strings consist of lowercase English letters only. The $i$-th letter of $a$ is $a_i$, the $i$-th letter of $b$ is $b_i$, the $i$-th letter of $c$ is $c_i$.</p><p>For every $i$ ($1 \leq i \leq n$) you <span class="tex-font-style-bf">must</span> swap (i.e. exchange) $c_i$ with either $a_i$ or $b_i$. So in total you'll perform exactly $n$ swap operations, each of them either $c_i \leftrightarrow a_i$ or $c_i \leftrightarrow b_i$ ($i$ iterates over all integers between $1$ and $n$, inclusive).</p><p>For example, if $a$ is "<span class="tex-font-style-tt">code</span>", $b$ is "<span class="tex-font-style-tt">true</span>", and $c$ is "<span class="tex-font-style-tt">help</span>", you can make $c$ equal to "<span class="tex-font-style-tt">crue</span>" taking the $1$-st and the $4$-th letters from $a$ and the others from $b$. In this way $a$ becomes "<span class="tex-font-style-tt">hodp</span>" and $b$ becomes "<span class="tex-font-style-tt">tele</span>".</p><p>Is it possible that after these swaps the string $a$ becomes exactly the same as the string $b$?</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a string of lowercase English letters $a$.</p><p>The second line of each test case contains a string of lowercase English letters $b$.</p><p>The third line of each test case contains a string of lowercase English letters $c$.</p><p>It is guaranteed that in each test case these three strings are non-empty and have the same length, which is not exceeding $100$.</p></div><div class="output-specification"><p>Print $t$ lines with answers for all test cases. For each test case:</p><p>If it is possible to make string $a$ equal to string $b$ print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print either lowercase or uppercase letters in the answers.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a string of lowercase English letters $a$.</p><p>The second line of each test case contains a string of lowercase English letters $b$.</p><p>The third line of each test case contains a string of lowercase English letters $c$.</p><p>It is guaranteed that in each test case these three strings are non-empty and have the same length, which is not exceeding $100$.</p>

## Output

<p>Print $t$ lines with answers for all test cases. For each test case:</p><p>If it is possible to make string $a$ equal to string $b$ print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print either lowercase or uppercase letters in the answers.</p>





```input1
4
aaa
bbb
ccc
abc
bca
bca
aabb
bbaa
baba
imi
mii
iim
```




```output1
NO
YES
YES
NO
```



## Note

<p>In the first test case, it is impossible to do the swaps so that string $a$ becomes exactly the same as string $b$.</p><p>In the second test case, you should swap $c_i$ with $a_i$ for all possible $i$. After the swaps $a$ becomes "<span class="tex-font-style-tt">bca</span>", $b$ becomes "<span class="tex-font-style-tt">bca</span>" and $c$ becomes "<span class="tex-font-style-tt">abc</span>". Here the strings $a$ and $b$ are equal.</p><p>In the third test case, you should swap $c_1$ with $a_1$, $c_2$ with $b_2$, $c_3$ with $b_3$ and $c_4$ with $a_4$. Then string $a$ becomes "<span class="tex-font-style-tt">baba</span>", string $b$ becomes "<span class="tex-font-style-tt">baba</span>" and string $c$ becomes "<span class="tex-font-style-tt">abab</span>". Here the strings $a$ and $b$ are equal.</p><p>In the fourth test case, it is impossible to do the swaps so that string $a$ becomes exactly the same as string $b$.</p>
