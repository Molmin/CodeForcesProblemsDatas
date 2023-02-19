## Description

<div><p>Right before the UEFA Euro 2020, AmShZ and Safar placed bets on who'd be the champion, AmShZ betting on Italy, and Safar betting on France.</p><p>Of course, AmShZ won. Hence, Safar gave him a bracket sequence $S$. Note that a bracket sequence is a string made of '(' and ')' characters.</p><p>AmShZ can perform the following operation any number of times:</p><ul> <li> First, he cuts his string $S$ into three (possibly empty) contiguous substrings $A, B$ and $C$. Then, he glues them back by using a '(' and a ')' characters, resulting in a new string $S$ = $A$ + "(" + $B$ + ")" + $C$.<p>For example, if $S$ = "))((" and AmShZ cuts it into $A$ = "", $B$ = "))", and $C$ = "((", He will obtain $S$ = "()))((" as a new string. </p></li></ul><p>After performing some (possibly none) operations, AmShZ gives his string to Keshi and asks him to find the initial string. Of course, Keshi might be able to come up with more than one possible initial string. Keshi is interested in finding the lexicographically smallest possible initial string.</p><p>Your task is to help Keshi in achieving his goal.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds:</p><ul><li> $a$ is a prefix of $b$, but $a \ne b$;</li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$.</li></ul></div><div class="input-specification"><p>The only line of input contains a single string $S$&nbsp;— the string after the operations $(1\le |S|\le 3 \cdot 10^5)$.</p><p>It is guaranteed that the first character of $S$ is ')'.</p></div><div class="output-specification"><p>Print the lexicographically smallest possible initial string before operations.</p></div>

## Input

<p>The only line of input contains a single string $S$&nbsp;— the string after the operations $(1\le |S|\le 3 \cdot 10^5)$.</p><p>It is guaranteed that the first character of $S$ is ')'.</p>

## Output

<p>Print the lexicographically smallest possible initial string before operations.</p>





```input1
)(()(())))
```




```output1
)((())))
```



## Note

<p>In the first sample, you can transform ")((())))" into ")(()(())))" by splitting it into ")(", empty string, and "(())))". It can be shown that this is the lexicographically smallest possible initial string</p>
