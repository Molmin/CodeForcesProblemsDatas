## Description

<div><p>You are given some text $t$ and a set of $n$ strings $s_1, s_2, \dots, s_n$. </p><p>In one step, you can choose any occurrence of any string $s_i$ in the text $t$ and color the corresponding characters of the text in red. For example, if $t=\texttt{bababa}$ and $s_1=\texttt{ba}$, $s_2=\texttt{aba}$, you can get $t=\color{red}{\texttt{ba}}\texttt{baba}$, $t=\texttt{b}\color{red}{\texttt{aba}}\texttt{ba}$ or $t=\texttt{bab}\color{red}{\texttt{aba}}$ in one step.</p><p>You want to color all the letters of the text $t$ in red. When you color a letter in red again, it stays red.</p><p>In the example above, three steps are enough:</p><ul> <li> Let's color $t[2 \dots 4]=s_2=\texttt{aba}$ in red, we get $t=\texttt{b}\color{red}{\texttt{aba}}\texttt{ba}$; </li><li> Let's color $t[1 \dots 2]=s_1=\texttt{ba}$ in red, we get $t=\color{red}{\texttt{baba}}\texttt{ba}$; </li><li> Let's color $t[4 \dots 6]=s_2=\texttt{aba}$ in red, we get $t=\color{red}{\texttt{bababa}}$. </li></ul><p>Each string $s_i$ can be applied any number of times (or not at all). Occurrences for coloring can intersect arbitrarily.</p><p>Determine the minimum number of steps needed to color all letters $t$ in red and how to do it. If it is impossible to color all letters of the text $t$ in red, output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line of the input contains an integer $q$ ($1 \le q \le 100$)&nbsp;—the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains the text $t$ ($1 \le |t| \le 100$), consisting only of lowercase Latin letters, where $|t|$ is the length of the text $t$.</p><p>The second line of each test case contains a single integer $n$ ($1 \le n \le 10$) — the number of strings in the set.</p><p>This is followed by $n$ lines, each containing a string $s_i$ ($1 \le |s_i| \le 10$) consisting only of lowercase Latin letters, where $|s_i|$&nbsp;— the length of string $s_i$.</p></div><div class="output-specification"><p>For each test case, print the answer on a separate line.</p><p>If it is impossible to color all the letters of the text in red, print a single line containing the number <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, on the first line, print the number $m$ — the minimum number of steps it will take to turn all the letters $t$ red.</p><p>Then in the next $m$ lines print pairs of indices: $w_j$ and $p_j$ ($1 \le j \le m$), which denote that the string with index $w_j$ was used as a substring to cover the occurrences starting in the text $t$ from position $p_j$. The pairs can be output in any order.</p><p>If there are several answers, output any of them.</p></div>

## Input

<p>The first line of the input contains an integer $q$ ($1 \le q \le 100$)&nbsp;—the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains the text $t$ ($1 \le |t| \le 100$), consisting only of lowercase Latin letters, where $|t|$ is the length of the text $t$.</p><p>The second line of each test case contains a single integer $n$ ($1 \le n \le 10$) — the number of strings in the set.</p><p>This is followed by $n$ lines, each containing a string $s_i$ ($1 \le |s_i| \le 10$) consisting only of lowercase Latin letters, where $|s_i|$&nbsp;— the length of string $s_i$.</p>

## Output

<p>For each test case, print the answer on a separate line.</p><p>If it is impossible to color all the letters of the text in red, print a single line containing the number <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, on the first line, print the number $m$ — the minimum number of steps it will take to turn all the letters $t$ red.</p><p>Then in the next $m$ lines print pairs of indices: $w_j$ and $p_j$ ($1 \le j \le m$), which denote that the string with index $w_j$ was used as a substring to cover the occurrences starting in the text $t$ from position $p_j$. The pairs can be output in any order.</p><p>If there are several answers, output any of them.</p>





```input1|2,3,4,5,10,11,12,13,14,20,21,22,23,24,25
6
bababa
2
ba
aba
caba
2
bac
acab
abacabaca
3
aba
bac
aca
baca
3
a
c
b
codeforces
4
def
code
efo
forces
aaaabbbbcccceeee
4
eeee
cccc
aaaa
bbbb
```




```output1
3
2 2
1 1
2 4
-1
4
1 1
2 6
3 3
3 7
4
3 1
1 2
2 3
1 4
2
4 5
2 1
4
3 1
4 5
2 9
1 13
```



## Note

<p>The first test case is explained in the problem statement.</p><p>In the second test case, it is impossible to color all the letters of the text in red.</p>
