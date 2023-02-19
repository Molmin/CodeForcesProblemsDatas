## Description

<div><p>You are given a string $s$, consisting only of Latin letters 'a', and a string $t$, consisting of lowercase Latin letters.</p><p>In one move, you can replace any letter 'a' in the string $s$ with a string $t$. Note that after the replacement string $s$ might contain letters other than 'a'.</p><p>You can perform an arbitrary number of moves (including zero). How many different strings can you obtain? Print the number, or report that it is infinitely large.</p><p>Two strings are considered different if they have different length, or they differ at some index.</p></div><div class="input-specification"><p>The first line contains a single integer $q$ ($1 \le q \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a non-empty string $s$, consisting only of Latin letters 'a'. The length of $s$ doesn't exceed $50$.</p><p>The second line contains a non-empty string $t$, consisting of lowercase Latin letters. The length of $t$ doesn't exceed $50$.</p></div><div class="output-specification"><p>For each testcase, print the number of different strings $s$ that can be obtained after an arbitrary amount of moves (including zero). If the number is infinitely large, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the number.</p></div>

## Input

<p>The first line contains a single integer $q$ ($1 \le q \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a non-empty string $s$, consisting only of Latin letters 'a'. The length of $s$ doesn't exceed $50$.</p><p>The second line contains a non-empty string $t$, consisting of lowercase Latin letters. The length of $t$ doesn't exceed $50$.</p>

## Output

<p>For each testcase, print the number of different strings $s$ that can be obtained after an arbitrary amount of moves (including zero). If the number is infinitely large, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the number.</p>





```input1
3
aaaa
a
aa
abc
a
b
```




```output1
1
-1
2
```



## Note

<p>In the first example, you can replace any letter 'a' with the string "a", but that won't change the string. So no matter how many moves you make, you can't obtain a string other than the initial one.</p><p>In the second example, you can replace the second letter 'a' with "abc". String $s$ becomes equal to "aabc". Then the second letter 'a' again. String $s$ becomes equal to "aabcbc". And so on, generating infinitely many different strings.</p><p>In the third example, you can either leave string $s$ as is, performing zero moves, or replace the only 'a' with "b". String $s$ becomes equal to "b", so you can't perform more moves on it.</p>
