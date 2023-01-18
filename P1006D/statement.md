## Description

<div><p>You are given two strings $a$ and $b$ consisting of lowercase English letters, both of length $n$. The characters of both strings have indices from $1$ to $n$, inclusive. </p><p>You are allowed to do the following <span class="tex-font-style-it">changes</span>: </p><ul> <li> Choose any index $i$ ($1 \le i \le n$) and swap characters $a_i$ and $b_i$; </li><li> Choose any index $i$ ($1 \le i \le n$) and swap characters $a_i$ and $a_{n - i + 1}$; </li><li> Choose any index $i$ ($1 \le i \le n$) and swap characters $b_i$ and $b_{n - i + 1}$. </li></ul><p>Note that if $n$ is odd, you are formally allowed to swap $a_{\lceil\frac{n}{2}\rceil}$ with $a_{\lceil\frac{n}{2}\rceil}$ (and the same with the string $b$) but this move is useless. Also you can swap two equal characters but this operation is useless as well.</p><p>You have to make these strings equal by applying any number of <span class="tex-font-style-it">changes</span> described above, in any order. But it is obvious that it may be impossible to make two strings equal by these swaps.</p><p>In one <span class="tex-font-style-it">preprocess move</span> you can replace a character in $a$ with another character. In other words, in a single <span class="tex-font-style-it">preprocess move</span> you can choose any index $i$ ($1 \le i \le n$), any character $c$ and set $a_i := c$.</p><p>Your task is to find the minimum number of <span class="tex-font-style-it">preprocess moves</span> to apply in such a way that after them you can make strings $a$ and $b$ equal by applying some number of <span class="tex-font-style-it">changes</span> described in the list above.</p><p>Note that the number of <span class="tex-font-style-it">changes</span> you make after the <span class="tex-font-style-it">preprocess moves</span> does not matter. Also note that you cannot apply <span class="tex-font-style-it">preprocess moves</span> to the string $b$ or make any <span class="tex-font-style-it">preprocess moves</span> after the first <span class="tex-font-style-it">change</span> is made.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 10^5$) — the length of strings $a$ and $b$.</p><p>The second line contains the string $a$ consisting of exactly $n$ lowercase English letters.</p><p>The third line contains the string $b$ consisting of exactly $n$ lowercase English letters.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of <span class="tex-font-style-it">preprocess moves</span> to apply before <span class="tex-font-style-it">changes</span>, so that it is possible to make the string $a$ equal to string $b$ with a sequence of <span class="tex-font-style-it">changes</span> from the list above.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 10^5$) — the length of strings $a$ and $b$.</p><p>The second line contains the string $a$ consisting of exactly $n$ lowercase English letters.</p><p>The third line contains the string $b$ consisting of exactly $n$ lowercase English letters.</p>

## Output

<p>Print a single integer — the minimum number of <span class="tex-font-style-it">preprocess moves</span> to apply before <span class="tex-font-style-it">changes</span>, so that it is possible to make the string $a$ equal to string $b$ with a sequence of <span class="tex-font-style-it">changes</span> from the list above.</p>





```input1
7
abacaba
bacabaa

```




```input2
5
zcabd
dbacz

```




```output1
4

```




```output2
0

```



## Note

<p>In the first example <span class="tex-font-style-it">preprocess moves</span> are as follows: $a_1 := $'<span class="tex-font-style-tt">b</span>', $a_3 := $'<span class="tex-font-style-tt">c</span>', $a_4 := $'<span class="tex-font-style-tt">a</span>' and $a_5:=$'<span class="tex-font-style-tt">b</span>'. Afterwards, $a = $"<span class="tex-font-style-tt">bbcabba</span>". Then we can obtain equal strings by the following sequence of <span class="tex-font-style-it">changes</span>: $swap(a_2, b_2)$ and $swap(a_2, a_6)$. There is no way to use fewer than $4$ <span class="tex-font-style-it">preprocess moves</span> before a sequence of <span class="tex-font-style-it">changes</span> to make string equal, so the answer in this example is $4$.</p><p>In the second example no <span class="tex-font-style-it">preprocess moves</span> are required. We can use the following sequence of <span class="tex-font-style-it">changes</span> to make $a$ and $b$ equal: $swap(b_1, b_5)$, $swap(a_2, a_4)$.</p>
