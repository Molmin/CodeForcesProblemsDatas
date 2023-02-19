## Description

<div><p>An integer array $a_1, a_2, \ldots, a_n$ is being transformed into an array of lowercase English letters using the following prodecure:</p><p>While there is at least one number in the array: </p><ul> <li> Choose any number $x$ from the array $a$, and any letter of the English alphabet $y$. </li><li> Replace all occurrences of number $x$ with the letter $y$. </li></ul><p>For example, if we initially had an array $a = [2, 3, 2, 4, 1]$, then we could transform it the following way:</p><ul> <li> Choose the number $2$ and the letter <span class="tex-font-style-tt">c</span>. After that $a = [c, 3, c, 4, 1]$. </li><li> Choose the number $3$ and the letter <span class="tex-font-style-tt">a</span>. After that $a = [c, a, c, 4, 1]$. </li><li> Choose the number $4$ and the letter <span class="tex-font-style-tt">t</span>. After that $a = [c, a, c, t, 1]$. </li><li> Choose the number $1$ and the letter <span class="tex-font-style-tt">a</span>. After that $a = [c, a, c, t, a]$. </li></ul><p>After the transformation all letters are united into a string, in our example we get the string "<span class="tex-font-style-tt">cacta</span>".</p><p>Having the array $a$ and the string $s$ determine if the string $s$ could be got from the array $a$ after the described transformation?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \leq t \leq 10^3$) — the number of test cases.</p><p>Then the description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 50$) — the length of the array $a$ and the string $s$.</p><p>The second line of each test case contains exactly $n$ integers: $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 50$) — the elements of the array $a$.</p><p>The third line of each test case contains a string $s$ of length $n$, consisting of lowercase English letters. </p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>", if we can get the string $s$ from the array $a$, and "<span class="tex-font-style-tt">NO</span>" otherwise. You can output each letter in any case.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \leq t \leq 10^3$) — the number of test cases.</p><p>Then the description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 50$) — the length of the array $a$ and the string $s$.</p><p>The second line of each test case contains exactly $n$ integers: $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 50$) — the elements of the array $a$.</p><p>The third line of each test case contains a string $s$ of length $n$, consisting of lowercase English letters. </p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>", if we can get the string $s$ from the array $a$, and "<span class="tex-font-style-tt">NO</span>" otherwise. You can output each letter in any case.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22
7
5
2 3 2 4 1
cacta
1
50
a
2
11 22
ab
4
1 2 2 1
aaab
5
1 2 3 2 1
aaaaa
6
1 10 2 9 3 8
azzfdb
7
1 2 3 4 1 1 2
abababb
```




```output1
YES
YES
YES
NO
YES
YES
NO
```



## Note

<p>The first test case corresponds to the sample described in the statement.</p><p>In the second test case we can choose the number $50$ and the letter <span class="tex-font-style-tt">a</span>.</p><p>In the third test case we can choose the number $11$ and the letter <span class="tex-font-style-tt">a</span>, after that $a = [a, 22]$. Then we choose the number $22$ and the letter <span class="tex-font-style-tt">b</span> and get $a = [a, b]$.</p><p>In the fifth test case we can change all numbers one by one to the letter <span class="tex-font-style-tt">a</span>.</p>
