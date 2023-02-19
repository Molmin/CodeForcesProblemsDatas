## Description

<div><p>Alina has discovered a weird language, which contains only $4$ words: $\texttt{A}$, $\texttt{B}$, $\texttt{AB}$, $\texttt{BA}$. It also turned out that there are no spaces in this language: a sentence is written by just concatenating its words into a single string.</p><p>Alina has found one such sentence $s$ and she is curious: is it possible that it consists of precisely $a$ words $\texttt{A}$, $b$ words $\texttt{B}$, $c$ words $\texttt{AB}$, and $d$ words $\texttt{BA}$?</p><p>In other words, determine, if it's possible to concatenate these $a+b+c+d$ words in some order so that the resulting string is $s$. Each of the $a+b+c+d$ words must be used exactly once in the concatenation, but you can choose the order in which they are concatenated.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains four integers $a$, $b$, $c$, $d$ ($0\le a,b,c,d\le 2\cdot 10^5$) — the number of times that words $\texttt{A}$, $\texttt{B}$, $\texttt{AB}$, $\texttt{BA}$ respectively must be used in the sentence.</p><p>The second line contains the string $s$ ($s$ consists only of the characters $\texttt{A}$ and $\texttt{B}$, $1\le |s| \le 2\cdot 10^5$, $|s|=a+b+2c+2d$) &nbsp;— the sentence. Notice that the condition $|s|=a+b+2c+2d$ (here $|s|$ denotes the length of the string $s$) is equivalent to the fact that $s$ is as long as the concatenation of the $a+b+c+d$ words.</p><p>The sum of the lengths of $s$ over all test cases doesn't exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output $\texttt{YES}$ if it is possible that the sentence $s$ consists of precisely $a$ words $\texttt{A}$, $b$ words $\texttt{B}$, $c$ words $\texttt{AB}$, and $d$ words $\texttt{BA}$, and $\texttt{NO}$ otherwise. You can output each letter in any case.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains four integers $a$, $b$, $c$, $d$ ($0\le a,b,c,d\le 2\cdot 10^5$) — the number of times that words $\texttt{A}$, $\texttt{B}$, $\texttt{AB}$, $\texttt{BA}$ respectively must be used in the sentence.</p><p>The second line contains the string $s$ ($s$ consists only of the characters $\texttt{A}$ and $\texttt{B}$, $1\le |s| \le 2\cdot 10^5$, $|s|=a+b+2c+2d$) &nbsp;— the sentence. Notice that the condition $|s|=a+b+2c+2d$ (here $|s|$ denotes the length of the string $s$) is equivalent to the fact that $s$ is as long as the concatenation of the $a+b+c+d$ words.</p><p>The sum of the lengths of $s$ over all test cases doesn't exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case output $\texttt{YES}$ if it is possible that the sentence $s$ consists of precisely $a$ words $\texttt{A}$, $b$ words $\texttt{B}$, $c$ words $\texttt{AB}$, and $d$ words $\texttt{BA}$, and $\texttt{NO}$ otherwise. You can output each letter in any case.</p>





```input1
8
1 0 0 0
B
0 0 1 0
AB
1 1 0 1
ABAB
1 0 1 1
ABAAB
1 1 2 2
BAABBABBAA
1 1 2 3
ABABABBAABAB
2 3 5 4
AABAABBABAAABABBABBBABB
1 3 3 10
BBABABABABBBABABABABABABAABABA
```




```output1
NO
YES
YES
YES
YES
YES
NO
YES
```



## Note

<p>In the first test case, the sentence $s$ is $\texttt{B}$. Clearly, it can't consist of a single word $\texttt{A}$, so the answer is $\texttt{NO}$.</p><p>In the second test case, the sentence $s$ is $\texttt{AB}$, and it's possible that it consists of a single word $\texttt{AB}$, so the answer is $\texttt{YES}$.</p><p>In the third test case, the sentence $s$ is $\texttt{ABAB}$, and it's possible that it consists of one word $\texttt{A}$, one word $\texttt{B}$, and one word $\texttt{BA}$, as $\texttt{A} + \texttt{BA} + \texttt{B} = \texttt{ABAB}$.</p><p>In the fourth test case, the sentence $s$ is $\texttt{ABAAB}$, and it's possible that it consists of one word $\texttt{A}$, one word $\texttt{AB}$, and one word $\texttt{BA}$, as $\texttt{A} + \texttt{BA} + \texttt{AB} = \texttt{ABAAB}$. </p><p>In the fifth test case, the sentence $s$ is $\texttt{BAABBABBAA}$, and it's possible that it consists of one word $\texttt{A}$, one word $\texttt{B}$, two words $\texttt{AB}$, and two words $\texttt{BA}$, as $\texttt{BA} + \texttt{AB} + \texttt{B} + \texttt{AB} + \texttt{BA} + \texttt{A}= \texttt{BAABBABBAA}$.</p>
