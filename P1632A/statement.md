## Description

<div><p>Recently, the students of School 179 have developed a unique algorithm, which takes in a binary string $s$ as input. However, they soon found out that if some substring $t$ of $s$ is a palindrome of length greater than <span class="tex-font-style-tt">1</span>, the algorithm will work incorrectly. Can the students somehow reorder the characters of $s$ so that the algorithm will work correctly on the string?</p><p>A binary string is a string where each character is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p><p>A palindrome is a string that reads the same backwards as forwards.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$) — the length of the string $s$.</p><p>The second line of each test case contains the string $s$ of length $n$ consisting only of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> (case-insensitive) if it is possible to reorder the characters of $s$ so that there are no substrings that are a palindrome of length greater than <span class="tex-font-style-tt">1</span>, or <span class="tex-font-style-tt">NO</span> (case-insensitive) otherwise.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$) — the length of the string $s$.</p><p>The second line of each test case contains the string $s$ of length $n$ consisting only of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> (case-insensitive) if it is possible to reorder the characters of $s$ so that there are no substrings that are a palindrome of length greater than <span class="tex-font-style-tt">1</span>, or <span class="tex-font-style-tt">NO</span> (case-insensitive) otherwise.</p>





```input1
4
1
1
2
10
2
01
4
1010
```




```output1
YES
YES
YES
NO
```



## Note

<p>In the first three test cases, the given strings do not contain palindromes of length greater than <span class="tex-font-style-tt">1</span>, so the answers are <span class="tex-font-style-tt">YES</span>.</p><p>In the last test case, it is impossible to reorder the characters so that the string does not contain palindromes of length greater than <span class="tex-font-style-tt">1</span>, so the answer is <span class="tex-font-style-tt">NO</span>.</p>
