## Description

<div><p>Serval soon said goodbye to Japari kindergarten, and began his life in Japari Primary School.</p><p>In his favorite math class, the teacher taught him the following interesting definitions.</p><p>A <span class="tex-font-style-it">parenthesis sequence</span> is a string, containing only characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p><p>A <span class="tex-font-style-it">correct parenthesis sequence</span> is a parenthesis sequence that can be transformed into a correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">+</span>" between the original characters of the sequence. For example, parenthesis sequences "<span class="tex-font-style-tt">()()</span>", "<span class="tex-font-style-tt">(())</span>" are correct (the resulting expressions are: "<span class="tex-font-style-tt">(1+1)+(1+1)</span>", "<span class="tex-font-style-tt">((1+1)+1)</span>"), while "<span class="tex-font-style-tt">)(</span>" and "<span class="tex-font-style-tt">)</span>" are not. Note that the empty string is a correct parenthesis sequence by definition.</p><p>We define that $|s|$ as the length of string $s$. A <span class="tex-font-style-it">strict prefix</span> $s[1\dots l]$ $(1\leq l&lt; |s|)$ of a string $s = s_1s_2\dots s_{|s|}$ is string $s_1s_2\dots s_l$. Note that the empty string and the whole string are not strict prefixes of any string by the definition.</p><p>Having learned these definitions, he comes up with a new problem. He writes down a string $s$ containing only characters "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>" and "<span class="tex-font-style-tt">?</span>". And what he is going to do, is to replace each of the "<span class="tex-font-style-tt">?</span>" in $s$ independently by one of "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" to make all strict prefixes of the new sequence not a correct parenthesis sequence, while the new sequence should be a correct parenthesis sequence.</p><p>After all, he is just a primary school student so this problem is too hard for him to solve. As his best friend, can you help him to replace the question marks? If there are many solutions, any of them is acceptable.</p></div><div class="input-specification"><p>The first line contains a single integer $|s|$ ($1\leq |s|\leq 3 \cdot 10^5$), the length of the string.</p><p>The second line contains a string $s$, containing only "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>" and "<span class="tex-font-style-tt">?</span>".</p></div><div class="output-specification"><p>A single line contains a string representing the answer.</p><p>If there are many solutions, any of them is acceptable.</p><p>If there is no answer, print a single line containing "<span class="tex-font-style-tt">:(</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a single integer $|s|$ ($1\leq |s|\leq 3 \cdot 10^5$), the length of the string.</p><p>The second line contains a string $s$, containing only "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>" and "<span class="tex-font-style-tt">?</span>".</p>

## Output

<p>A single line contains a string representing the answer.</p><p>If there are many solutions, any of them is acceptable.</p><p>If there is no answer, print a single line containing "<span class="tex-font-style-tt">:(</span>" (without the quotes).</p>





```input1
6
(?????
```




```input2
10
(???(???(?
```




```output1
(()())
```




```output2
:(
```



## Note

<p>It can be proved that there is no solution for the second sample, so print "<span class="tex-font-style-tt">:(</span>".</p>
