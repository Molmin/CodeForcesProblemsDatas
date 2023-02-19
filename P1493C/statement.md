## Description

<div><p>You are given a string $s$ consisting of lowercase English letters and a number $k$. Let's call a string consisting of lowercase English letters <span class="tex-font-style-it">beautiful</span> if the number of occurrences of each letter in that string is divisible by $k$. You are asked to find the lexicographically smallest beautiful string of length $n$, which is lexicographically greater or equal to string $s$. If such a string does not exist, output $-1$.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds: </p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 10\,000$) — the number of test cases.</p><p>The next $2 \cdot T$ lines contain the description of test cases. The description of each test case consists of two lines.</p><p>The first line of the description contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$) — the length of string $s$ and number $k$ respectively.</p><p>The second line contains string $s$ consisting of lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case output in a separate line lexicographically smallest beautiful string of length $n$, which is greater or equal to string $s$, or $-1$ if such a string does not exist.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 10\,000$) — the number of test cases.</p><p>The next $2 \cdot T$ lines contain the description of test cases. The description of each test case consists of two lines.</p><p>The first line of the description contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$) — the length of string $s$ and number $k$ respectively.</p><p>The second line contains string $s$ consisting of lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case output in a separate line lexicographically smallest beautiful string of length $n$, which is greater or equal to string $s$, or $-1$ if such a string does not exist.</p>





```input1
4
4 2
abcd
3 1
abc
4 3
aaaa
9 3
abaabaaaa
```




```output1
acac
abc
-1
abaabaaab
```



## Note

<p>In the first test case "<span class="tex-font-style-tt">acac</span>" is greater than or equal to $s$, and each letter appears $2$ or $0$ times in it, so it is beautiful.</p><p>In the second test case each letter appears $0$ or $1$ times in $s$, so $s$ itself is the answer.</p><p>We can show that there is no suitable string in the third test case.</p><p>In the fourth test case each letter appears $0$, $3$, or $6$ times in "<span class="tex-font-style-tt">abaabaaab</span>". All these integers are divisible by $3$.</p>
