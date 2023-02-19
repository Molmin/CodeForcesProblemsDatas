## Description

<div><p>Timur initially had a binary string$^{\dagger}$ $s$ (possibly of length $0$). He performed the following operation several (possibly zero) times: </p><ul> <li> Add $\texttt{0}$ to one end of the string and $\texttt{1}$ to the other end of the string. For example, starting from the string $\texttt{1011}$, you can obtain either $\color{red}{\texttt{0}}\texttt{1011}\color{red}{\texttt{1}}$ or $\color{red}{\texttt{1}}\texttt{1011}\color{red}{\texttt{0}}$. </li></ul> You are given Timur's final string. What is the length of the <span class="tex-font-style-bf">shortest</span> possible string he could have started with?<p>$^{\dagger}$ A binary string is a string (possibly the empty string) whose characters are either $\texttt{0}$ or $\texttt{1}$.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2000$)&nbsp;— the length of Timur's final string.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of characters $\texttt{0}$ or $\texttt{1}$, denoting the final string.</p></div><div class="output-specification"><p>For each test case, output a single nonnegative integer&nbsp;— the shortest possible length of Timur's original string. Note that Timur's original string could have been empty, in which case you should output $0$.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2000$)&nbsp;— the length of Timur's final string.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of characters $\texttt{0}$ or $\texttt{1}$, denoting the final string.</p>

## Output

<p>For each test case, output a single nonnegative integer&nbsp;— the shortest possible length of Timur's original string. Note that Timur's original string could have been empty, in which case you should output $0$.</p>





```input1|2,3,6,7,10,11,14,15,18,19
9
3
100
4
0111
5
10101
6
101010
7
1010110
1
1
2
10
2
11
10
1011011010
```




```output1
1
2
5
0
3
1
0
2
4
```



## Note

<p>In the first test case, the shortest possible string Timur started with is $\texttt{0}$, and he performed the following operation: $\texttt{0} \to \color{red}{\texttt{1}}\texttt{0}\color{red}{\texttt{0}}$.</p><p>In the second test case, the shortest possible string Timur started with is $\texttt{11}$, and he performed the following operation: $\texttt{11} \to \color{red}{\texttt{0}}\texttt{11}\color{red}{\texttt{1}}$.</p><p>In the third test case, the shortest possible string Timur started with is $\texttt{10101}$, and he didn't perform any operations.</p><p>In the fourth test case, the shortest possible string Timur started with is the empty string (which we denote by $\varepsilon$), and he performed the following operations: $\varepsilon \to \color{red}{\texttt{1}}\texttt{}\color{red}{\texttt{0}} \to \color{red}{\texttt{0}}\texttt{10}\color{red}{\texttt{1}} \to \color{red}{\texttt{1}}\texttt{0101}\color{red}{\texttt{0}}$.</p><p>In the fifth test case, the shortest possible string Timur started with is $\texttt{101}$, and he performed the following operations: $\texttt{101} \to \color{red}{\texttt{0}}\texttt{101}\color{red}{\texttt{1}} \to \color{red}{\texttt{1}}\texttt{01011}\color{red}{\texttt{0}}$.</p>
