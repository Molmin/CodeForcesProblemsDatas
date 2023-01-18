## Description

<div><p>The Little Girl loves problems on games very much. Here's one of them.</p><p>Two players have got a string <span class="tex-span"><i>s</i></span>, consisting of lowercase English letters. They play a game that is described by the following rules:</p><ul> <li> The players move in turns; In one move the player can remove an arbitrary letter from string <span class="tex-span"><i>s</i></span>. </li><li> If the player before his turn can reorder the letters in string <span class="tex-span"><i>s</i></span> so as to get a palindrome, this player wins. A palindrome is a string that reads the same both ways (from left to right, and vice versa). For example, string "<span class="tex-font-style-tt">abba</span>" is a palindrome and string "<span class="tex-font-style-tt">abc</span>" isn't. </li></ul><p>Determine which player will win, provided that both sides play optimally well — the one who moves first or the one who moves second.</p></div><div class="input-specification"><p>The input contains a single line, containing string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>|  ≤  10<sup class="upper-index">3</sup></span>). String <span class="tex-span"><i>s</i></span> consists of lowercase English letters.</p></div><div class="output-specification"><p>In a single line print word "<span class="tex-font-style-tt">First</span>" if the first player wins (provided that both players play optimally well). Otherwise, print word "<span class="tex-font-style-tt">Second</span>". Print the words without the quotes.</p></div>

## Input

<p>The input contains a single line, containing string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>|  ≤  10<sup class="upper-index">3</sup></span>). String <span class="tex-span"><i>s</i></span> consists of lowercase English letters.</p>

## Output

<p>In a single line print word "<span class="tex-font-style-tt">First</span>" if the first player wins (provided that both players play optimally well). Otherwise, print word "<span class="tex-font-style-tt">Second</span>". Print the words without the quotes.</p>





```input1
aba

```




```input2
abca

```




```output1
First

```




```output2
Second

```


