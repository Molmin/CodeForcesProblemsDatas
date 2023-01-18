## Description

<div><p>Vasya has a string $s$ of length $n$ consisting only of digits <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. Also he has an array $a$ of length $n$. </p><p>Vasya performs the following operation until the string becomes empty: choose some <span class="tex-font-style-bf">consecutive</span> substring of <span class="tex-font-style-bf">equal characters</span>, erase it from the string and glue together the remaining parts (any of them can be empty). For example, if he erases substring <span class="tex-font-style-tt">111</span> from string <span class="tex-font-style-tt">1<span class="tex-font-style-bf">111</span>10</span> he will get the string <span class="tex-font-style-tt">110</span>. Vasya gets $a_x$ points for erasing substring of length $x$.</p><p>Vasya wants to maximize his total points, so help him with this! </p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 100$) — the length of string $s$.</p><p>The second line contains string $s$, consisting only of digits <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The third line contains $n$ integers $a_1, a_2, \dots a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the number of points for erasing the substring of length $i$.</p></div><div class="output-specification"><p>Print one integer — the maximum total points Vasya can get.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 100$) — the length of string $s$.</p><p>The second line contains string $s$, consisting only of digits <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The third line contains $n$ integers $a_1, a_2, \dots a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the number of points for erasing the substring of length $i$.</p>

## Output

<p>Print one integer — the maximum total points Vasya can get.</p>





```input1
7
1101001
3 4 9 100 1 2 3
```




```input2
5
10101
3 10 15 15 15
```




```output1
109
```




```output2
23
```



## Note

<p>In the first example the optimal sequence of erasings is: <span class="tex-font-style-tt">11<span class="tex-font-style-bf">0</span>1001</span> $\rightarrow$ <span class="tex-font-style-tt">1110<span class="tex-font-style-bf">0</span>1</span> $\rightarrow$ <span class="tex-font-style-tt">111<span class="tex-font-style-bf">0</span>1</span> $\rightarrow$ <span class="tex-font-style-tt"><span class="tex-font-style-bf">1111</span></span> $\rightarrow$ $\varnothing$.</p><p>In the second example the optimal sequence of erasings is: <span class="tex-font-style-tt">10<span class="tex-font-style-bf">1</span>01</span> $\rightarrow$ <span class="tex-font-style-tt">1<span class="tex-font-style-bf">00</span>1</span> $\rightarrow$ <span class="tex-font-style-tt"><span class="tex-font-style-bf">11</span></span> $\rightarrow$ $\varnothing$.</p>
