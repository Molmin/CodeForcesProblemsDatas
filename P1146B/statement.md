## Description

<div><p>Bob has a string $s$ consisting of lowercase English letters. He defines $s'$ to be the string after removing all "<span class="tex-font-style-tt">a</span>" characters from $s$ (keeping all other characters in the same order). He then generates a new string $t$ by concatenating $s$ and $s'$. In other words, $t=s+s'$ (look at notes for an example).</p><p>You are given a string $t$. Your task is to find some $s$ that Bob could have used to generate $t$. It can be shown that if an answer exists, it will be unique.</p></div><div class="input-specification"><p>The first line of input contains a string $t$ ($1 \leq |t| \leq 10^5$) consisting of lowercase English letters.</p></div><div class="output-specification"><p>Print a string $s$ that could have generated $t$. It can be shown if an answer exists, it is unique. If no string exists, print "<span class="tex-font-style-tt">:(</span>" (without double quotes, there is no space between the characters).</p></div>

## Input

<p>The first line of input contains a string $t$ ($1 \leq |t| \leq 10^5$) consisting of lowercase English letters.</p>

## Output

<p>Print a string $s$ that could have generated $t$. It can be shown if an answer exists, it is unique. If no string exists, print "<span class="tex-font-style-tt">:(</span>" (without double quotes, there is no space between the characters).</p>





```input1
aaaaa
```




```input2
aacaababc
```




```input3
ababacacbbcc
```




```input4
baba
```




```output1
aaaaa
```




```output2
:(
```




```output3
ababacac
```




```output4
:(
```



## Note

<p>In the first example, we have $s = $ "<span class="tex-font-style-tt">aaaaa</span>", and $s' = $ "<span class="tex-font-style-tt"></span>".</p><p>In the second example, no such $s$ can work that will generate the given $t$.</p><p>In the third example, we have $s = $ "<span class="tex-font-style-tt">ababacac</span>", and $s' = $ "<span class="tex-font-style-tt">bbcc</span>", and $t = s + s' = $ "<span class="tex-font-style-tt">ababacacbbcc</span>".</p>
