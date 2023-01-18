## Description

<div><p>A telephone number is a sequence of <span class="tex-font-style-bf">exactly</span> $11$ digits such that its first digit is <span class="tex-font-style-tt">8</span>.</p><p>Vasya and Petya are playing a game. Initially they have a string $s$ of length $n$ ($n$ is odd) consisting of digits. Vasya makes the first move, then players alternate turns. In one move the player <span class="tex-font-style-bf">must</span> choose a character and erase it from the current string. For example, if the current string <span class="tex-font-style-tt">1121</span>, after the player's move it may be <span class="tex-font-style-tt">112</span>, <span class="tex-font-style-tt">111</span> or <span class="tex-font-style-tt">121</span>. The game ends when the length of string $s$ becomes <span class="tex-font-style-tt">11</span>. If the resulting string is a telephone number, Vasya wins, otherwise Petya wins.</p><p>You have to determine if Vasya has a winning strategy (that is, if Vasya can win the game no matter which characters Petya chooses during his moves).</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($13 \le n &lt; 10^5$, $n$ is odd) — the length of string $s$.</p><p>The second line contains the string $s$ ($|s| = n$) consisting only of decimal digits.</p></div><div class="output-specification"><p>If Vasya has a strategy that guarantees him victory, print <span class="tex-font-style-tt">YES</span>.</p><p>Otherwise print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer $n$ ($13 \le n &lt; 10^5$, $n$ is odd) — the length of string $s$.</p><p>The second line contains the string $s$ ($|s| = n$) consisting only of decimal digits.</p>

## Output

<p>If Vasya has a strategy that guarantees him victory, print <span class="tex-font-style-tt">YES</span>.</p><p>Otherwise print <span class="tex-font-style-tt">NO</span>.</p>





```input1
13
8380011223344
```




```input2
15
807345619350641
```




```output1
YES
```




```output2
NO
```



## Note

<p>In the first example Vasya needs to erase the second character. Then Petya cannot erase a character from the remaining string <span class="tex-font-style-tt">880011223344</span> so that it does not become a telephone number.</p><p>In the second example after Vasya's turn Petya can erase one character character <span class="tex-font-style-tt">8</span>. The resulting string can't be a telephone number, because there is no digit <span class="tex-font-style-tt">8</span> at all.</p>
