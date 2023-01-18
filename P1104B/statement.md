## Description

<div><p>Two people are playing a game with a string $s$, consisting of lowercase latin letters. </p><p>On a player's turn, he should choose two consecutive equal letters in the string and delete them. </p><p>For example, if the string is equal to "<span class="tex-font-style-tt">xaax</span>" than there is only one possible turn: delete "<span class="tex-font-style-tt">aa</span>", so the string will become "<span class="tex-font-style-tt">xx</span>". A player not able to make a turn loses.</p><p>Your task is to determine which player will win if both play optimally.</p></div><div class="input-specification"><p>The only line contains the string $s$, consisting of lowercase latin letters ($1 \leq |s| \leq 100\,000$), where $|s|$ means the length of a string $s$.</p></div><div class="output-specification"><p>If the first player wins, print "<span class="tex-font-style-tt">Yes</span>". If the second player wins, print "<span class="tex-font-style-tt">No</span>".</p></div>

## Input

<p>The only line contains the string $s$, consisting of lowercase latin letters ($1 \leq |s| \leq 100\,000$), where $|s|$ means the length of a string $s$.</p>

## Output

<p>If the first player wins, print "<span class="tex-font-style-tt">Yes</span>". If the second player wins, print "<span class="tex-font-style-tt">No</span>".</p>





```input1
abacaba
```




```input2
iiq
```




```input3
abba
```




```output1
No
```




```output2
Yes
```




```output3
No
```



## Note

<p>In the first example the first player is unable to make a turn, so he loses.</p><p>In the second example first player turns the string into "<span class="tex-font-style-tt">q</span>", then second player is unable to move, so he loses.</p>
