## Description

<div><p>Homer has two friends Alice and Bob. Both of them are string fans. </p><p>One day, Alice and Bob decide to play a game on a string $s = s_1 s_2 \dots s_n$ of length $n$ consisting of lowercase English letters. They move in turns alternatively and <span class="tex-font-style-bf">Alice makes the first move</span>.</p><p>In a move, a player <span class="tex-font-style-bf">must</span> choose an index $i$ ($1 \leq i \leq n$) that has not been chosen before, and change $s_i$ to any other lowercase English letter $c$ that $c \neq s_i$.</p><p>When all indices have been chosen, the game ends. </p><p>The goal of Alice is to make the final string lexicographically as small as possible, while the goal of Bob is to make the final string lexicographically as large as possible. Both of them are game experts, so they always play games optimally. Homer is not a game expert, so he wonders what the final string will be.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds: </p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases. Description of the test cases follows.</p><p>The only line of each test case contains a single string $s$ ($1 \leq |s| \leq 50$) consisting of lowercase English letters.</p></div><div class="output-specification"><p>For each test case, print the final string in a single line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases. Description of the test cases follows.</p><p>The only line of each test case contains a single string $s$ ($1 \leq |s| \leq 50$) consisting of lowercase English letters.</p>

## Output

<p>For each test case, print the final string in a single line.</p>





```input1
3
a
bbbb
az
```




```output1
b
azaz
by
```



## Note

<p>In the first test case: Alice makes the first move and must change the only letter to a different one, so she changes it to '<span class="tex-font-style-tt">b</span>'.</p><p>In the second test case: Alice changes the first letter to '<span class="tex-font-style-tt">a</span>', then Bob changes the second letter to '<span class="tex-font-style-tt">z</span>', Alice changes the third letter to '<span class="tex-font-style-tt">a</span>' and then Bob changes the fourth letter to '<span class="tex-font-style-tt">z</span>'.</p><p>In the third test case: Alice changes the first letter to '<span class="tex-font-style-tt">b</span>', and then Bob changes the second letter to '<span class="tex-font-style-tt">y</span>'.</p>
