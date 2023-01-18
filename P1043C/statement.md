## Description

<div><p>IA has so many colorful magnets on her fridge! Exactly one letter is written on each magnet, '<span class="tex-font-style-tt">a</span>' or '<span class="tex-font-style-tt">b</span>'. She loves to play with them, placing all magnets in a row. However, the girl is quickly bored and usually thinks how to make her entertainment more interesting.</p><p>Today, when IA looked at the fridge, she noticed that the word formed by magnets is really messy. "It would look much better when I'll swap some of them!"&nbsp;— thought the girl&nbsp;— "but how to do it?". After a while, she got an idea. IA will look at all prefixes with lengths from $1$ to the length of the word and for each prefix she will either reverse this prefix or leave it as it is. She will consider the prefixes in the fixed order: from the shortest to the largest. She wants to get the lexicographically smallest possible word after she considers all prefixes. Can you help her, telling which prefixes should be chosen for reversing?</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds:</p><ul><li> $a$ is a prefix of $b$, but $a \ne b$;</li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$.</li></ul></div><div class="input-specification"><p>The first and the only line contains a string $s$ ($1 \le |s| \le 1000$), describing the initial string formed by magnets. The string $s$ consists only of characters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p></div><div class="output-specification"><p>Output exactly $|s|$ integers. If IA should reverse the $i$-th prefix (that is, the substring from $1$ to $i$), the $i$-th integer should be equal to $1$, and it should be equal to $0$ otherwise.</p><p>If there are multiple possible sequences leading to the optimal answer, print any of them.</p></div>

## Input

<p>The first and the only line contains a string $s$ ($1 \le |s| \le 1000$), describing the initial string formed by magnets. The string $s$ consists only of characters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'.</p>

## Output

<p>Output exactly $|s|$ integers. If IA should reverse the $i$-th prefix (that is, the substring from $1$ to $i$), the $i$-th integer should be equal to $1$, and it should be equal to $0$ otherwise.</p><p>If there are multiple possible sequences leading to the optimal answer, print any of them.</p>





```input1
bbab

```




```input2
aaaaa

```




```output1
0 1 1 0

```




```output2
1 0 0 0 1

```



## Note

<p>In the first example, IA can reverse the second and the third prefix and get a string "<span class="tex-font-style-tt">abbb</span>". She cannot get better result, since it is also lexicographically smallest string obtainable by permuting characters of the initial string.</p><p>In the second example, she can reverse any subset of prefixes&nbsp;— all letters are '<span class="tex-font-style-tt">a</span>'.</p>
