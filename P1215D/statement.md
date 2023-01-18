## Description

<div><p>Monocarp and Bicarp live in Berland, where every bus ticket consists of $n$ digits ($n$ is an even number). During the evening walk Monocarp and Bicarp found a ticket where some of the digits have been erased. <span class="tex-font-style-bf">The number of digits that have been erased is even</span>.</p><p>Monocarp and Bicarp have decided to play a game with this ticket. Monocarp hates happy tickets, while Bicarp collects them. A ticket is considered happy if the sum of the first $\frac{n}{2}$ digits of this ticket is equal to the sum of the last $\frac{n}{2}$ digits.</p><p>Monocarp and Bicarp take turns (and Monocarp performs the first of them). During each turn, the current player must replace any erased digit with any digit from $0$ to $9$. The game ends when there are no erased digits in the ticket.</p><p>If the ticket is happy after all erased digits are replaced with decimal digits, then Bicarp wins. Otherwise, Monocarp wins. You have to determine who will win if both players play optimally.</p></div><div class="input-specification"><p>The first line contains one <span class="tex-font-style-bf">even</span> integer $n$ $(2 \le n \le 2 \cdot 10^{5})$ — the number of digits in the ticket.</p><p>The second line contains a string of $n$ digits and "<span class="tex-font-style-tt">?</span>" characters — the ticket which Monocarp and Bicarp have found. If the $i$-th character is "<span class="tex-font-style-tt">?</span>", then the $i$-th digit is erased. Note that there may be leading zeroes. The number of "<span class="tex-font-style-tt">?</span>" characters is even.</p></div><div class="output-specification"><p>If Monocarp wins, print "<span class="tex-font-style-tt">Monocarp</span>" (without quotes). Otherwise print "<span class="tex-font-style-tt">Bicarp</span>" (without quotes).</p></div>

## Input

<p>The first line contains one <span class="tex-font-style-bf">even</span> integer $n$ $(2 \le n \le 2 \cdot 10^{5})$ — the number of digits in the ticket.</p><p>The second line contains a string of $n$ digits and "<span class="tex-font-style-tt">?</span>" characters — the ticket which Monocarp and Bicarp have found. If the $i$-th character is "<span class="tex-font-style-tt">?</span>", then the $i$-th digit is erased. Note that there may be leading zeroes. The number of "<span class="tex-font-style-tt">?</span>" characters is even.</p>

## Output

<p>If Monocarp wins, print "<span class="tex-font-style-tt">Monocarp</span>" (without quotes). Otherwise print "<span class="tex-font-style-tt">Bicarp</span>" (without quotes).</p>





```input1
4
0523
```




```input2
2
??
```




```input3
8
?054??0?
```




```input4
6
???00?
```




```output1
Bicarp
```




```output2
Bicarp
```




```output3
Bicarp
```




```output4
Monocarp
```



## Note

<p>Since there is no question mark in the ticket in the first example, the winner is determined before the game even starts, and it is Bicarp.</p><p>In the second example, Bicarp also wins. After Monocarp chooses an erased digit and replaces it with a new one, Bicap can choose another position with an erased digit and replace it with the same digit, so the ticket is happy.</p>
