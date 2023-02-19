## Description

<div><p>Polycarp has a string $s$ consisting of lowercase Latin letters.</p><p>He encodes it using the following algorithm.</p><p>He goes through the letters of the string $s$ from left to right and for each letter Polycarp considers its number in the alphabet:</p><ul> <li> if the letter number is single-digit number (less than $10$), then just writes it out; </li><li> if the letter number is a two-digit number (greater than or equal to $10$), then it writes it out and adds the number <span class="tex-font-style-tt">0</span> after. </li></ul><p>For example, if the string $s$ is <span class="tex-font-style-tt">code</span>, then Polycarp will encode this string as follows:</p><ul> <li> '<span class="tex-font-style-tt">c</span>'&nbsp;— is the $3$-rd letter of the alphabet. Consequently, Polycarp adds <span class="tex-font-style-tt">3</span> to the code (the code becomes equal to <span class="tex-font-style-tt">3</span>); </li><li> '<span class="tex-font-style-tt">o</span>'&nbsp;— is the $15$-th letter of the alphabet. Consequently, Polycarp adds <span class="tex-font-style-tt">15</span> to the code and also <span class="tex-font-style-tt">0</span> (the code becomes <span class="tex-font-style-tt">3150</span>); </li><li> '<span class="tex-font-style-tt">d</span>'&nbsp;— is the $4$-th letter of the alphabet. Consequently, Polycarp adds <span class="tex-font-style-tt">4</span> to the code (the code becomes <span class="tex-font-style-tt">31504</span>); </li><li> '<span class="tex-font-style-tt">e</span>'&nbsp;— is the $5$-th letter of the alphabet. Therefore, Polycarp adds <span class="tex-font-style-tt">5</span> to the code (the code becomes <span class="tex-font-style-tt">315045</span>). </li></ul><p>Thus, code of string <span class="tex-font-style-tt">code</span> is <span class="tex-font-style-tt">315045</span>.</p><p>You are given a string $t$ resulting from encoding the string $s$. Your task is to decode it (get the original string $s$ by $t$).</p></div><div class="input-specification"><p>The first line of the input contains an integer $q$ ($1 \le q \le 10^4$) — the number of test cases in the input.</p><p>The descriptions of the test cases follow.</p><p>The first line of description of each test case contains one integer $n$ ($1 \le n \le 50$) — the length of the given code.</p><p>The second line of the description of each test case contains a string $t$ of length $n$ — the given code. It is guaranteed that there exists such a string of lowercase Latin letters, as a result of encoding which the string $t$ is obtained.</p></div><div class="output-specification"><p>For each test case output the required string $s$ — the string that gives string $t$ as the result of encoding. It is guaranteed that such a string always exists. It can be shown that such a string is always unique.</p></div>

## Input

<p>The first line of the input contains an integer $q$ ($1 \le q \le 10^4$) — the number of test cases in the input.</p><p>The descriptions of the test cases follow.</p><p>The first line of description of each test case contains one integer $n$ ($1 \le n \le 50$) — the length of the given code.</p><p>The second line of the description of each test case contains a string $t$ of length $n$ — the given code. It is guaranteed that there exists such a string of lowercase Latin letters, as a result of encoding which the string $t$ is obtained.</p>

## Output

<p>For each test case output the required string $s$ — the string that gives string $t$ as the result of encoding. It is guaranteed that such a string always exists. It can be shown that such a string is always unique.</p>





```input1|2,3,6,7,10,11,14,15,18,19
9
6
315045
4
1100
7
1213121
6
120120
18
315045615018035190
7
1111110
7
1111100
5
11111
4
2606
```




```output1
code
aj
abacaba
ll
codeforces
aaaak
aaaaj
aaaaa
zf
```



## Note

<p>The first test case is explained above.</p><p>In the second test case, the answer is <span class="tex-font-style-tt">aj</span>. Indeed, the number of the letter <span class="tex-font-style-tt">a</span> is equal to $1$, so <span class="tex-font-style-tt">1</span> will be appended to the code. The number of the letter <span class="tex-font-style-tt">j</span> is $10$, so <span class="tex-font-style-tt">100</span> will be appended to the code. The resulting code is <span class="tex-font-style-tt">1100</span>.</p><p>There are no zeros in the third test case, which means that the numbers of all letters are less than $10$ and are encoded as one digit. The original string is <span class="tex-font-style-tt">abacaba</span>.</p><p>In the fourth test case, the string $s$ is equal to <span class="tex-font-style-tt">ll</span>. The letter <span class="tex-font-style-tt">l</span> has the number $12$ and is encoded as <span class="tex-font-style-tt">120</span>. So <span class="tex-font-style-tt">ll</span> is indeed <span class="tex-font-style-tt">120120</span>.</p>
