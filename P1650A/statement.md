## Description

<div><p>The string $s$ is given, the string length is <span class="tex-font-style-bf">odd</span> number. The string consists of lowercase letters of the Latin alphabet.</p><p>As long as the string length is greater than $1$, the following operation can be performed on it: select any two adjacent letters in the string $s$ and delete them from the string. For example, from the string "<span class="tex-font-style-tt">lemma</span>" in one operation, you can get any of the four strings: "<span class="tex-font-style-tt">mma</span>", "<span class="tex-font-style-tt">lma</span>", "<span class="tex-font-style-tt">lea</span>" or "<span class="tex-font-style-tt">lem</span>" In particular, in one operation, the length of the string reduces by $2$.</p><p>Formally, let the string $s$ have the form $s=s_1s_2 \dots s_n$ ($n&gt;1$). During one operation, you choose an arbitrary index $i$ ($1 \le i &lt; n$) and replace $s=s_1s_2 \dots s_{i-1}s_{i+2} \dots s_n$.</p><p>For the given string $s$ and the letter $c$, determine whether it is possible to make such a sequence of operations that in the end the equality $s=c$ will be true? In other words, is there such a sequence of operations that the process will end with a string of length $1$, which consists of the letter $c$?</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 10^3$) — the number of input test cases.</p><p>The descriptions of the $t$ cases follow. Each test case is represented by two lines:</p><ul> <li> string $s$, which has an odd length from $1$ to $49$ inclusive and consists of lowercase letters of the Latin alphabet; </li><li> is a string containing one letter $c$, where $c$ is a lowercase letter of the Latin alphabet. </li></ul></div><div class="output-specification"><p>For each test case in a separate line output:</p><ul> <li><span class="tex-font-style-tt">YES</span>, if the string $s$ can be converted so that $s=c$ is true; </li><li><span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 10^3$) — the number of input test cases.</p><p>The descriptions of the $t$ cases follow. Each test case is represented by two lines:</p><ul> <li> string $s$, which has an odd length from $1$ to $49$ inclusive and consists of lowercase letters of the Latin alphabet; </li><li> is a string containing one letter $c$, where $c$ is a lowercase letter of the Latin alphabet. </li></ul>

## Output

<p>For each test case in a separate line output:</p><ul> <li><span class="tex-font-style-tt">YES</span>, if the string $s$ can be converted so that $s=c$ is true; </li><li><span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p>





```input1
5
abcde
c
abcde
b
x
y
aaaaaaaaaaaaaaa
a
contest
t
```




```output1
YES
NO
NO
YES
YES
```



## Note

<p>In the first test case, $s$="<span class="tex-font-style-tt">abcde</span>". You need to get $s$="<span class="tex-font-style-tt">c</span>". For the first operation, delete the first two letters, we get $s$="<span class="tex-font-style-tt">cde</span>". In the second operation, we delete the last two letters, so we get the expected value of $s$="<span class="tex-font-style-tt">c</span>".</p><p>In the third test case, $s$="<span class="tex-font-style-tt">x</span>", it is required to get $s$="<span class="tex-font-style-tt">y</span>". Obviously, this cannot be done.</p>
