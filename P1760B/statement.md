## Description

<div><p>In order to write a string, Atilla needs to first learn all letters that are contained in the string.</p><p>Atilla needs to write a message which can be represented as a string $s$. He asks you what is the minimum alphabet size required so that one can write this message.</p><p>The alphabet of size $x$ ($1 \leq x \leq 26$) contains <span class="tex-font-style-bf">only the first</span> $x$ Latin letters. For example an alphabet of size $4$ contains <span class="tex-font-style-bf">only</span> the characters $\texttt{a}$, $\texttt{b}$, $\texttt{c}$ and $\texttt{d}$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;— the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the minimum alphabet size required to so that Atilla can write his message $s$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;— the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of lowercase Latin letters.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the minimum alphabet size required to so that Atilla can write his message $s$.</p>





```input1|2,3,6,7,10,11
5
1
a
4
down
10
codeforces
3
bcf
5
zzzzz
```




```output1
1
23
19
6
26
```



## Note

<p>For the first test case, Atilla needs to know only the character $\texttt{a}$, so the alphabet of size $1$ which only contains $\texttt{a}$ is enough.</p><p>For the second test case, Atilla needs to know the characters $\texttt{d}$, $\texttt{o}$, $\texttt{w}$, $\texttt{n}$. The smallest alphabet size that contains all of them is $23$ (such alphabet can be represented as the string $\texttt{abcdefghijklmnopqrstuvw}$).</p>
