## Description

<div><p>Alice has a string $s$. She really likes the letter "<span class="tex-font-style-tt">a</span>". She calls a string good if strictly more than half of the characters in that string are "<span class="tex-font-style-tt">a</span>"s. For example "<span class="tex-font-style-tt">aaabb</span>", "<span class="tex-font-style-tt">axaa</span>" are good strings, and "<span class="tex-font-style-tt">baca</span>", "<span class="tex-font-style-tt">awwwa</span>", "" (empty string) are not.</p><p>Alice can erase some characters from her string $s$. She would like to know what is the longest string remaining after erasing some characters (possibly zero) to get a good string. It is guaranteed that the string has at least one "<span class="tex-font-style-tt">a</span>" in it, so the answer always exists.</p></div><div class="input-specification"><p>The first line contains a string $s$ ($1 \leq |s| \leq 50$) consisting of lowercase English letters. It is guaranteed that there is at least one "<span class="tex-font-style-tt">a</span>" in $s$.</p></div><div class="output-specification"><p>Print a single integer, the length of the longest good string that Alice can get after erasing some characters from $s$.</p></div>

## Input

<p>The first line contains a string $s$ ($1 \leq |s| \leq 50$) consisting of lowercase English letters. It is guaranteed that there is at least one "<span class="tex-font-style-tt">a</span>" in $s$.</p>

## Output

<p>Print a single integer, the length of the longest good string that Alice can get after erasing some characters from $s$.</p>





```input1
xaxxxxa
```




```input2
aaabaa
```




```output1
3
```




```output2
6
```



## Note

<p>In the first example, it's enough to erase any four of the "<span class="tex-font-style-tt">x</span>"s. The answer is $3$ since that is the maximum number of characters that can remain.</p><p>In the second example, we don't need to erase any characters.</p>
