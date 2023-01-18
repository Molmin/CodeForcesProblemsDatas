## Description

<div><p>Consider all binary strings of length $m$ ($1 \le m \le 60$). A binary string is a string that consists of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span> only. For example, <span class="tex-font-style-tt">0110</span> is a binary string, and <span class="tex-font-style-tt">012aba</span> is not. Obviously, there are exactly $2^m$ such strings in total.</p><p>The string $s$ is lexicographically smaller than the string $t$ (both have the same length $m$) if in the first position $i$ from the left in which they differ, we have $s[i] &lt; t[i]$. This is exactly the way strings are compared in dictionaries and in most modern programming languages when comparing them in a standard way. For example, the string <span class="tex-font-style-tt">01011</span> is lexicographically smaller than the string <span class="tex-font-style-tt">01100</span>, because the first two characters are the same, and the third character in the first string is less than that in the second.</p><p>We remove from this set $n$ ($1 \le n \le \min(2^m-1, 100)$) <span class="tex-font-style-bf">distinct</span> binary strings $a_1, a_2, \ldots, a_n$, each of length $m$. Thus, the set will have $k=2^m-n$ strings. Sort all strings of the resulting set in lexicographical ascending order (as in the dictionary).</p><p>We number all the strings after sorting from $0$ to $k-1$. Print the string whose index is $\lfloor \frac{k-1}{2} \rfloor$ (such an element is called <span class="tex-font-style-it">median</span>), where $\lfloor x \rfloor$ is the rounding of the number down to the nearest integer.</p><p>For example, if $n=3$, $m=3$ and $a=[$<span class="tex-font-style-tt">010</span>, <span class="tex-font-style-tt">111</span>, <span class="tex-font-style-tt">001</span>$]$, then after removing the strings $a_i$ and sorting, the result will take the form: $[$<span class="tex-font-style-tt">000</span>, <span class="tex-font-style-tt">011</span>, <span class="tex-font-style-tt">100</span>, <span class="tex-font-style-tt">101</span>, <span class="tex-font-style-tt">110</span>$]$. Thus, the desired median is <span class="tex-font-style-tt">100</span>.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Then, $t$ test cases follow.</p><p>The first line of each test case contains integers $n$ ($1 \le n \le \min(2^m-1, 100)$) and $m$ ($1 \le m \le 60$), where $n$ is the number of strings to remove, and $m$ is the length of binary strings. The next $n$ lines contain $a_1, a_2, \ldots, a_n$&nbsp;— <span class="tex-font-style-bf">distinct</span> binary strings of length $m$.</p><p>The total length of all given binary strings in all test cases in one test does not exceed $10^5$.</p></div><div class="output-specification"><p>Print $t$ answers to the test cases. For each test case, print a string of length $m$&nbsp;— the median of the sorted sequence of remaining strings in the corresponding test case.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Then, $t$ test cases follow.</p><p>The first line of each test case contains integers $n$ ($1 \le n \le \min(2^m-1, 100)$) and $m$ ($1 \le m \le 60$), where $n$ is the number of strings to remove, and $m$ is the length of binary strings. The next $n$ lines contain $a_1, a_2, \ldots, a_n$&nbsp;— <span class="tex-font-style-bf">distinct</span> binary strings of length $m$.</p><p>The total length of all given binary strings in all test cases in one test does not exceed $10^5$.</p>

## Output

<p>Print $t$ answers to the test cases. For each test case, print a string of length $m$&nbsp;— the median of the sorted sequence of remaining strings in the corresponding test case.</p>





```input1
5
3 3
010
001
111
4 3
000
111
100
011
1 1
1
1 1
0
3 2
00
01
10
```




```output1
100
010
0
1
11
```



## Note

<p>The first test case is explained in the statement.</p><p>In the second test case, the result after removing strings and sorting is $[$<span class="tex-font-style-tt">001</span>, <span class="tex-font-style-tt">010</span>, <span class="tex-font-style-tt">101</span>, <span class="tex-font-style-tt">110</span>$]$. Therefore, the desired median is <span class="tex-font-style-tt">010</span>.</p>
