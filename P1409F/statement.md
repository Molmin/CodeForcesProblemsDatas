## Description

<div><p>You are given two strings $s$ and $t$ consisting of lowercase Latin letters. The length of $t$ is $2$ (i.e. this string consists only of two characters).</p><p>In one move, you can choose <span class="tex-font-style-bf">any</span> character of $s$ and replace it with <span class="tex-font-style-bf">any</span> lowercase Latin letter. More formally, you choose some $i$ and replace $s_i$ (the character at the position $i$) with some character from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>'.</p><p>You want to do <span class="tex-font-style-bf">no more than</span> $k$ replacements in such a way that <span class="tex-font-style-bf">maximizes</span> the number of occurrences of $t$ in $s$ as a <span class="tex-font-style-bf">subsequence</span>.</p><p>Recall that a subsequence is a sequence that can be derived from the given sequence by deleting zero or more elements without changing the order of the remaining elements.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($2 \le n \le 200$; $0 \le k \le n$) — the length of $s$ and the maximum number of moves you can make. The second line of the input contains the string $s$ consisting of $n$ lowercase Latin letters. The third line of the input contains the string $t$ consisting of two lowercase Latin letters.</p></div><div class="output-specification"><p>Print one integer — the maximum possible number of occurrences of $t$ in $s$ as a <span class="tex-font-style-bf">subsequence</span> if you replace no more than $k$ characters in $s$ optimally.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($2 \le n \le 200$; $0 \le k \le n$) — the length of $s$ and the maximum number of moves you can make. The second line of the input contains the string $s$ consisting of $n$ lowercase Latin letters. The third line of the input contains the string $t$ consisting of two lowercase Latin letters.</p>

## Output

<p>Print one integer — the maximum possible number of occurrences of $t$ in $s$ as a <span class="tex-font-style-bf">subsequence</span> if you replace no more than $k$ characters in $s$ optimally.</p>





```input1
4 2
bbaa
ab
```




```input2
7 3
asddsaf
sd
```




```input3
15 6
qwertyhgfdsazxc
qa
```




```input4
7 2
abacaba
aa
```




```output1
3
```




```output2
10
```




```output3
16
```




```output4
15
```



## Note

<p>In the first example, you can obtain the string "<span class="tex-font-style-tt">abab</span>" replacing $s_1$ with '<span class="tex-font-style-tt">a</span>' and $s_4$ with '<span class="tex-font-style-tt">b</span>'. Then the answer is $3$.</p><p>In the second example, you can obtain the string "<span class="tex-font-style-tt">ssddsdd</span>" and get the answer $10$.</p><p>In the fourth example, you can obtain the string "<span class="tex-font-style-tt">aaacaaa</span>" and get the answer $15$.</p>
