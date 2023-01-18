## Description

<div><p>Phoenix has a string $s$ consisting of lowercase Latin letters. He wants to distribute all the letters of his string into $k$ <span class="tex-font-style-bf">non-empty</span> strings $a_1, a_2, \dots, a_k$ such that every letter of $s$ goes to exactly one of the strings $a_i$. The strings $a_i$ <span class="tex-font-style-bf">do not</span> need to be substrings of $s$. Phoenix can distribute letters of $s$ and rearrange the letters within each string $a_i$ however he wants.</p><p>For example, if $s = $ <span class="tex-font-style-tt">baba</span> and $k=2$, Phoenix may distribute the letters of his string in many ways, such as: </p><ul> <li> <span class="tex-font-style-tt">ba</span> and <span class="tex-font-style-tt">ba</span> </li><li> <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">abb</span> </li><li> <span class="tex-font-style-tt">ab</span> and <span class="tex-font-style-tt">ab</span> </li><li> <span class="tex-font-style-tt">aa</span> and <span class="tex-font-style-tt">bb</span> </li></ul><p>But these ways are invalid: </p><ul> <li> <span class="tex-font-style-tt">baa</span> and <span class="tex-font-style-tt">ba</span> </li><li> <span class="tex-font-style-tt">b</span> and <span class="tex-font-style-tt">ba</span> </li><li> <span class="tex-font-style-tt">baba</span> and empty string ($a_i$ should be non-empty) </li></ul><p>Phoenix wants to distribute the letters of his string $s$ into $k$ strings $a_1, a_2, \dots, a_k$ to <span class="tex-font-style-bf">minimize</span> the lexicographically maximum string among them, i.&nbsp;e. minimize $max(a_1, a_2, \dots, a_k)$. Help him find the optimal distribution and print the minimal possible value of $max(a_1, a_2, \dots, a_k)$.</p><p>String $x$ is lexicographically less than string $y$ if either $x$ is a prefix of $y$ and $x \ne y$, or there exists an index $i$ ($1 \le i \le min(|x|, |y|))$ such that $x_i$ &lt; $y_i$ and for every $j$ $(1 \le j &lt; i)$ $x_j = y_j$. Here $|x|$ denotes the length of the string $x$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Each test case consists of two lines.</p><p>The first line of each test case consists of two integers $n$ and $k$ ($1 \le k \le n \le 10^5$)&nbsp;— the length of string $s$ and the number of non-empty strings, into which Phoenix wants to distribute letters of $s$, respectively.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting only of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases is $\le 10^5$.</p></div><div class="output-specification"><p>Print $t$ answers&nbsp;— one per test case. The $i$-th answer should be the minimal possible value of $max(a_1, a_2, \dots, a_k)$ in the $i$-th test case.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Each test case consists of two lines.</p><p>The first line of each test case consists of two integers $n$ and $k$ ($1 \le k \le n \le 10^5$)&nbsp;— the length of string $s$ and the number of non-empty strings, into which Phoenix wants to distribute letters of $s$, respectively.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting only of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases is $\le 10^5$.</p>

## Output

<p>Print $t$ answers&nbsp;— one per test case. The $i$-th answer should be the minimal possible value of $max(a_1, a_2, \dots, a_k)$ in the $i$-th test case.</p>





```input1
6
4 2
baba
5 2
baacb
5 3
baacb
5 3
aaaaa
6 4
aaxxzz
7 1
phoenix
```




```output1
ab
abbc
b
aa
x
ehinopx
```



## Note

<p>In the first test case, one optimal solution is to distribute <span class="tex-font-style-tt">baba</span> into <span class="tex-font-style-tt">ab</span> and <span class="tex-font-style-tt">ab</span>. </p><p>In the second test case, one optimal solution is to distribute <span class="tex-font-style-tt">baacb</span> into <span class="tex-font-style-tt">abbc</span> and <span class="tex-font-style-tt">a</span>.</p><p>In the third test case, one optimal solution is to distribute <span class="tex-font-style-tt">baacb</span> into <span class="tex-font-style-tt">ac</span>, <span class="tex-font-style-tt">ab</span>, and <span class="tex-font-style-tt">b</span>.</p><p>In the fourth test case, one optimal solution is to distribute <span class="tex-font-style-tt">aaaaa</span> into <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">aa</span>, and <span class="tex-font-style-tt">a</span>.</p><p>In the fifth test case, one optimal solution is to distribute <span class="tex-font-style-tt">aaxxzz</span> into <span class="tex-font-style-tt">az</span>, <span class="tex-font-style-tt">az</span>, <span class="tex-font-style-tt">x</span>, and <span class="tex-font-style-tt">x</span>.</p><p>In the sixth test case, one optimal solution is to distribute <span class="tex-font-style-tt">phoenix</span> into <span class="tex-font-style-tt">ehinopx</span>.</p>
