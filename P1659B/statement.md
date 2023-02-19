## Description

<div><p>You are given a binary string of length $n$. You have <span class="tex-font-style-bf">exactly</span> $k$ moves. In one move, you must select a single bit. The state of all bits <span class="tex-font-style-bf">except</span> that bit will get flipped ($0$ becomes $1$, $1$ becomes $0$). You need to output the lexicographically largest string that you can get after using <span class="tex-font-style-bf">all</span> $k$ moves. Also, output the number of times you will select each bit. If there are multiple ways to do this, you may output any of them.</p><p>A binary string $a$ is lexicographically larger than a binary string $b$ of the same length, if and only if the following holds: </p><ul> <li> in the first position where $a$ and $b$ differ, the string $a$ contains a $1$, and the string $b$ contains a $0$. </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases.</p><p>Each test case has two lines. The first line has two integers $n$ and $k$ ($1 \leq n \leq 2 \cdot 10^5$; $0 \leq k \leq 10^9$).</p><p>The second line has a binary string of length $n$, each character is either $0$ or $1$.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output two lines.</p><p>The first line should contain the lexicographically largest string you can obtain.</p><p>The second line should contain $n$ integers $f_1, f_2, \ldots, f_n$, where $f_i$ is the number of times the $i$-th bit is selected. The sum of all the integers <span class="tex-font-style-bf">must be equal to</span> $k$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases.</p><p>Each test case has two lines. The first line has two integers $n$ and $k$ ($1 \leq n \leq 2 \cdot 10^5$; $0 \leq k \leq 10^9$).</p><p>The second line has a binary string of length $n$, each character is either $0$ or $1$.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output two lines.</p><p>The first line should contain the lexicographically largest string you can obtain.</p><p>The second line should contain $n$ integers $f_1, f_2, \ldots, f_n$, where $f_i$ is the number of times the $i$-th bit is selected. The sum of all the integers <span class="tex-font-style-bf">must be equal to</span> $k$.</p>





```input1
6
6 3
100001
6 4
100011
6 0
000000
6 1
111001
6 11
101100
6 12
001110
```




```output1
111110
1 0 0 2 0 0 
111110
0 1 1 1 0 1 
000000
0 0 0 0 0 0 
100110
1 0 0 0 0 0 
111111
1 2 1 3 0 4 
111110
1 1 4 2 0 4
```



## Note

<p>Here is the explanation for the first testcase. Each step shows how the binary string changes in a move.</p><ul> <li> Choose bit $1$: $\color{red}{\underline{1}00001} \rightarrow \color{red}{\underline{1}}\color{blue}{11110}$. </li><li> Choose bit $4$: $\color{red}{111\underline{1}10} \rightarrow \color{blue}{000}\color{red}{\underline{1}}\color{blue}{01}$. </li><li> Choose bit $4$: $\color{red}{000\underline{1}01} \rightarrow \color{blue}{111}\color{red}{\underline{1}}\color{blue}{10}$. </li></ul> The final string is $111110$ and this is the lexicographically largest string we can get.
