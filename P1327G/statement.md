## Description

<div><p>You are given a string $S$ and an array of strings $[t_1, t_2, \dots, t_k]$. Each string $t_i$ consists of lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">n</span>; $S$ consists of lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">n</span> and <span class="tex-font-style-bf">no more than $14$</span> question marks.</p><p>Each string $t_i$ has its cost $c_i$ — an integer number. The value of some string $T$ is calculated as $\sum\limits_{i = 1}^{k} F(T, t_i) \cdot c_i$, where $F(T, t_i)$ is the number of occurences of string $t_i$ in $T$ as a substring. For example, $F(\text{aaabaaa}, \text{aa}) = 4$.</p><p>You have to replace all question marks in $S$ with <span class="tex-font-style-bf">pairwise distinct</span> lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">n</span> so the value of $S$ is maximum possible.</p></div><div class="input-specification"><p>The first line contains one integer $k$ ($1 \le k \le 1000$) — the number of strings in the array $[t_1, t_2, \dots, t_k]$.</p><p>Then $k$ lines follow, each containing one string $t_i$ (consisting of lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">n</span>) and one integer $c_i$ ($1 \le |t_i| \le 1000$, $-10^6 \le c_i \le 10^6$). The sum of lengths of all strings $t_i$ does not exceed $1000$.</p><p>The last line contains one string $S$ ($1 \le |S| \le 4 \cdot 10^5$) consisting of lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">n</span> and question marks. The number of question marks in $S$ is not greater than $14$.</p></div><div class="output-specification"><p>Print one integer — the maximum value of $S$ after replacing all question marks with <span class="tex-font-style-bf">pairwise distinct</span> lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">n</span>.</p></div>

## Input

<p>The first line contains one integer $k$ ($1 \le k \le 1000$) — the number of strings in the array $[t_1, t_2, \dots, t_k]$.</p><p>Then $k$ lines follow, each containing one string $t_i$ (consisting of lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">n</span>) and one integer $c_i$ ($1 \le |t_i| \le 1000$, $-10^6 \le c_i \le 10^6$). The sum of lengths of all strings $t_i$ does not exceed $1000$.</p><p>The last line contains one string $S$ ($1 \le |S| \le 4 \cdot 10^5$) consisting of lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">n</span> and question marks. The number of question marks in $S$ is not greater than $14$.</p>

## Output

<p>Print one integer — the maximum value of $S$ after replacing all question marks with <span class="tex-font-style-bf">pairwise distinct</span> lowercase Latin letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">n</span>.</p>





```input1
4
abc -10
a 1
b 1
c 3
?b?
```




```input2
2
a 1
a 1
?
```




```input3
3
a 1
b 3
ab 4
ab
```




```input4
1
a -1
?????????????
```




```input5
1
a -1
??????????????
```




```output1
5
```




```output2
2
```




```output3
8
```




```output4
0
```




```output5
-1
```


