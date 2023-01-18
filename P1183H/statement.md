## Description

<div><p><span class="tex-font-style-bf">The only difference between the easy and the hard versions is constraints</span>.</p><p>A subsequence is a string that can be derived from another string by deleting some or no symbols without changing the order of the remaining symbols. Characters to be deleted are not required to go successively, there can be any gaps between them. For example, for the string "<span class="tex-font-style-tt">abaca</span>" the following strings are subsequences: "<span class="tex-font-style-tt">abaca</span>", "<span class="tex-font-style-tt">aba</span>", "<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt"></span>" (empty string). But the following strings are not subsequences: "<span class="tex-font-style-tt">aabaca</span>", "<span class="tex-font-style-tt">cb</span>" and "<span class="tex-font-style-tt">bcaa</span>".</p><p>You are given a string $s$ consisting of $n$ lowercase Latin letters.</p><p>In one move you can take <span class="tex-font-style-bf">any</span> subsequence $t$ of the given string and add it to the set $S$. The set $S$ can't contain duplicates. This move costs $n - |t|$, where $|t|$ is the length of the added subsequence (i.e. the price equals to the number of the deleted characters).</p><p>Your task is to find out the minimum possible total cost to obtain a set $S$ of size $k$ or report that it is impossible to do so.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 100, 1 \le k \le 10^{12}$) — the length of the string and the size of the set, correspondingly.</p><p>The second line of the input contains a string $s$ consisting of $n$ lowercase Latin letters.</p></div><div class="output-specification"><p>Print one integer — if it is impossible to obtain the set $S$ of size $k$, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum possible total cost to do it.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 100, 1 \le k \le 10^{12}$) — the length of the string and the size of the set, correspondingly.</p><p>The second line of the input contains a string $s$ consisting of $n$ lowercase Latin letters.</p>

## Output

<p>Print one integer — if it is impossible to obtain the set $S$ of size $k$, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum possible total cost to do it.</p>





```input1
4 5
asdf
```




```input2
5 6
aaaaa
```




```input3
5 7
aaaaa
```




```input4
10 100
ajihiushda
```




```output1
4
```




```output2
15
```




```output3
-1
```




```output4
233
```



## Note

<p>In the first example we can generate $S$ = { "<span class="tex-font-style-tt">asdf</span>", "<span class="tex-font-style-tt">asd</span>", "<span class="tex-font-style-tt">adf</span>", "<span class="tex-font-style-tt">asf</span>", "<span class="tex-font-style-tt">sdf</span>" }. The cost of the first element in $S$ is $0$ and the cost of the others is $1$. So the total cost of $S$ is $4$.</p>
