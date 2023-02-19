## Description

<div><p>Today is an important day for chef Tonio — an auditor has arrived in his hometown of Morioh. He has also arrived at Tonio's restaurant and ordered dessert. Tonio has not been prepared for this turn of events.</p><p>As you know, dessert is a string of lowercase English letters. Tonio remembered the rule of desserts&nbsp;— a string $s$ of length $n$. Any dessert $t$ is <span class="tex-font-style-it">delicious</span> if the number of occurrences of $t$ in $s$ as a substring is <span class="tex-font-style-bf">divisible</span> by the length of $t$.</p><p>Now Tonio wants to know the number of delicious substrings of $s$. If the substring occurs several times in the string $s$, then all occurrences must be taken into account.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \leq n \leq 10^6$) — the length of the rule $s$.</p><p>The second line contains the string $s$ of length $n$ — the rule. The rule consists only of lowercase English letters.</p></div><div class="output-specification"><p>In a single line print the number of delicious substrings of $s$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \leq n \leq 10^6$) — the length of the rule $s$.</p><p>The second line contains the string $s$ of length $n$ — the rule. The rule consists only of lowercase English letters.</p>

## Output

<p>In a single line print the number of delicious substrings of $s$.</p>





```input1
7
abacaba
```




```input2
8
abaababa
```




```input3
10
deadinside
```




```input4
5
aaaaa
```




```output1
11
```




```output2
11
```




```output3
12
```




```output4
12
```



## Note

<p>In the first sample, there are many delicious substrings. $7$ of them are substrings of length $1$ (<span class="tex-font-style-it">because any number is divisible by $1$</span>). Consider other delicious substrings:</p><ul> <li> "<span class="tex-font-style-tt">ab</span>" occurs in $s$ $2$ times, which is divisible by the length of the substring. </li><li> "<span class="tex-font-style-tt">ba</span>" also occurs $2$ times. </li></ul><p>Therefore, the answer is $7 + 2 + 2 = 11$.</p><p>Note that the answer includes both occurrences of "<span class="tex-font-style-tt">ab</span>" and "<span class="tex-font-style-tt">ba</span>".</p>
