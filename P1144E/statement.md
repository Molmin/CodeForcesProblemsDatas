## Description

<div><p>You are given two strings $s$ and $t$, both consisting of exactly $k$ lowercase Latin letters, $s$ is lexicographically less than $t$.</p><p>Let's consider list of all strings consisting of exactly $k$ lowercase Latin letters, lexicographically not less than $s$ and not greater than $t$ (including $s$ and $t$) in lexicographical order. For example, for $k=2$, $s=$"<span class="tex-font-style-tt">az</span>" and $t=$"<span class="tex-font-style-tt">bf</span>" the list will be ["<span class="tex-font-style-tt">az</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">bb</span>", "<span class="tex-font-style-tt">bc</span>", "<span class="tex-font-style-tt">bd</span>", "<span class="tex-font-style-tt">be</span>", "<span class="tex-font-style-tt">bf</span>"].</p><p>Your task is to print the median (the middle element) of this list. For the example above this will be "<span class="tex-font-style-tt">bc</span>".</p><p><span class="tex-font-style-bf">It is guaranteed that there is an odd number of strings lexicographically not less than $s$ and not greater than $t$</span>.</p></div><div class="input-specification"><p>The first line of the input contains one integer $k$ ($1 \le k \le 2 \cdot 10^5$) — the length of strings.</p><p>The second line of the input contains one string $s$ consisting of exactly $k$ lowercase Latin letters.</p><p>The third line of the input contains one string $t$ consisting of exactly $k$ lowercase Latin letters.</p><p>It is guaranteed that $s$ is lexicographically less than $t$.</p><p><span class="tex-font-style-bf">It is guaranteed that there is an odd number of strings lexicographically not less than $s$ and not greater than $t$</span>.</p></div><div class="output-specification"><p>Print one string consisting exactly of $k$ lowercase Latin letters — the median (the middle element) of list of strings of length $k$ lexicographically not less than $s$ and not greater than $t$.</p></div>

## Input

<p>The first line of the input contains one integer $k$ ($1 \le k \le 2 \cdot 10^5$) — the length of strings.</p><p>The second line of the input contains one string $s$ consisting of exactly $k$ lowercase Latin letters.</p><p>The third line of the input contains one string $t$ consisting of exactly $k$ lowercase Latin letters.</p><p>It is guaranteed that $s$ is lexicographically less than $t$.</p><p><span class="tex-font-style-bf">It is guaranteed that there is an odd number of strings lexicographically not less than $s$ and not greater than $t$</span>.</p>

## Output

<p>Print one string consisting exactly of $k$ lowercase Latin letters — the median (the middle element) of list of strings of length $k$ lexicographically not less than $s$ and not greater than $t$.</p>





```input1
2
az
bf
```




```input2
5
afogk
asdji
```




```input3
6
nijfvj
tvqhwp
```




```output1
bc
```




```output2
alvuw
```




```output3
qoztvz
```


