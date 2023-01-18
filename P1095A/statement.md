## Description

<div><p>Polycarp loves ciphers. He has invented his own cipher called <span class="tex-font-style-it">repeating</span>.</p><p>Repeating cipher is used for strings. To encrypt the string $s=s_{1}s_{2} \dots s_{m}$ ($1 \le m \le 10$), Polycarp uses the following algorithm:</p><ul> <li> he writes down $s_1$ ones, </li><li> he writes down $s_2$ twice, </li><li> he writes down $s_3$ three times, </li><li> ... </li><li> he writes down $s_m$ $m$ times. </li></ul><p>For example, if $s$="<span class="tex-font-style-tt">bab</span>" the process is: "<span class="tex-font-style-tt">b</span>" $\to$ "<span class="tex-font-style-tt">baa</span>" $\to$ "<span class="tex-font-style-tt">baabbb</span>". So the encrypted $s$="<span class="tex-font-style-tt">bab</span>" is "<span class="tex-font-style-tt">baabbb</span>".</p><p>Given string $t$ — the result of encryption of some string $s$. Your task is to decrypt it, i. e. find the string $s$.</p></div><div class="input-specification"><p>The first line contains integer $n$ ($1 \le n \le 55$) — the length of the encrypted string. The second line of the input contains $t$ — the result of encryption of some string $s$. It contains only lowercase Latin letters. The length of $t$ is exactly $n$.</p><p>It is guaranteed that the answer to the test exists.</p></div><div class="output-specification"><p>Print such string $s$ that after encryption it equals $t$.</p></div>

## Input

<p>The first line contains integer $n$ ($1 \le n \le 55$) — the length of the encrypted string. The second line of the input contains $t$ — the result of encryption of some string $s$. It contains only lowercase Latin letters. The length of $t$ is exactly $n$.</p><p>It is guaranteed that the answer to the test exists.</p>

## Output

<p>Print such string $s$ that after encryption it equals $t$.</p>





```input1
6
baabbb
```




```input2
10
ooopppssss
```




```input3
1
z
```




```output1
bab
```




```output2
oops
```




```output3
z
```


