## Description

<div><p>The development of a text editor is a hard problem. You need to implement an extra module for brackets coloring in text.</p><p>Your editor consists of a line with infinite length and cursor, which points to the current character. Please note that it points to only one of the characters (and not between a pair of characters). Thus, it points to an index character. The user can move the cursor left or right one position. If the cursor is already at the first (leftmost) position, then it does not move left.</p><p>Initially, the cursor is in the first (leftmost) character.</p><p>Also, the user can write a letter or brackets (either <span class="tex-font-style-tt">(</span>, or <span class="tex-font-style-tt">)</span>) to the position that the cursor is currently pointing at. A new character always overwrites the old value at that position.</p><p>Your editor must check, whether the current line is the <span class="tex-font-style-tt">correct text</span>. Text is correct if the brackets in them form the <span class="tex-font-style-it">correct bracket sequence</span>.</p><p>Formally, correct text (CT) must satisfy the following rules: </p><ul> <li> any line without brackets is CT (the line can contain whitespaces); </li><li> If the first character of the string — is <span class="tex-font-style-tt">(</span>, the last — is <span class="tex-font-style-tt">)</span>, and all the rest form a CT, then the whole line is a CT; </li><li> two consecutively written CT is also CT. </li></ul><p>Examples of correct texts: <span class="tex-font-style-tt">hello(codeforces)</span>, <span class="tex-font-style-tt">round</span>, <span class="tex-font-style-tt">((i)(write))edi(tor)s</span>, <span class="tex-font-style-tt">( me)</span>. Examples of incorrect texts: <span class="tex-font-style-tt">hello)oops(</span>, <span class="tex-font-style-tt">round)</span>, <span class="tex-font-style-tt">((me)</span>.</p><p>The user uses special commands to work with your editor. Each command has its symbol, which must be written to execute this command.</p><p>The correspondence of commands and characters is as follows: </p><ul> <li> <span class="tex-font-style-tt">L</span> — move the cursor one character to the left (remains in place if it already points to the first character); </li><li> <span class="tex-font-style-tt">R</span> — move the cursor one character to the right; </li><li> any lowercase Latin letter or bracket (<span class="tex-font-style-tt">(</span> or <span class="tex-font-style-tt">)</span>) — write the entered character to the position where the cursor is now. </li></ul><p>For a complete understanding, take a look at the first example and its illustrations in the note below.</p><p>You are given a string containing the characters that the user entered. For the brackets coloring module's work, after each command you need to:</p><ul> <li> check if the current text in the editor is a correct text; </li><li> if it is, print the least number of colors that required, to color all brackets. </li></ul><p>If two pairs of brackets are nested (the first in the second or vice versa), then these pairs of brackets should be painted in <span class="tex-font-style-it">different</span> colors. If two pairs of brackets are not nested, then they can be painted in different or the same colors. For example, for the bracket sequence <span class="tex-font-style-tt">()(())()()</span> the least number of colors is $2$, and for the bracket sequence <span class="tex-font-style-tt">(()(()())())(())</span> — is $3$.</p><p>Write a program that prints the minimal number of colors after processing each command.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 10^6$) — the number of commands. </p><p>The second line contains $s$ — a sequence of commands. The string $s$ consists of $n$ characters. It is guaranteed that all characters in a string are valid commands.</p></div><div class="output-specification"><p>In a single line print $n$ integers, where the $i$-th number is:</p><ul> <li> $-1$ if the line received after processing the first $i$ commands is not valid text, </li><li> the minimal number of colors in the case of the correct text. </li></ul></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 10^6$) — the number of commands. </p><p>The second line contains $s$ — a sequence of commands. The string $s$ consists of $n$ characters. It is guaranteed that all characters in a string are valid commands.</p>

## Output

<p>In a single line print $n$ integers, where the $i$-th number is:</p><ul> <li> $-1$ if the line received after processing the first $i$ commands is not valid text, </li><li> the minimal number of colors in the case of the correct text. </li></ul>





```input1
11
(RaRbR)L)L(
```




```input2
11
(R)R(R)Ra)c
```




```output1
-1 -1 -1 -1 -1 -1 1 1 -1 -1 2
```




```output2
-1 -1 1 1 -1 -1 1 1 1 -1 1
```



## Note

<p>In the first example, the text in the editor will take the following form:</p><ol> <li> <pre class="verbatim">(<br>^</pre> </li><li> <pre class="verbatim">(<br> ^</pre> </li><li> <pre class="verbatim">(a<br> ^</pre> </li><li> <pre class="verbatim">(a<br>  ^</pre> </li><li> <pre class="verbatim">(ab<br>  ^</pre> </li><li> <pre class="verbatim">(ab<br>   ^</pre> </li><li> <pre class="verbatim">(ab)<br>   ^</pre> </li><li> <pre class="verbatim">(ab)<br>  ^</pre> </li><li> <pre class="verbatim">(a))<br>  ^</pre> </li><li> <pre class="verbatim">(a))<br> ^</pre> </li><li> <pre class="verbatim">(())<br> ^</pre> </li></ol>
