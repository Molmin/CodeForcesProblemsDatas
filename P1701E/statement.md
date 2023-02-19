## Description

<div><p>You wanted to write a text $t$ consisting of $m$ lowercase Latin letters. But instead, you have written a text $s$ consisting of $n$ lowercase Latin letters, and now you want to fix it by obtaining the text $t$ from the text $s$.</p><p>Initially, the cursor of your text editor is at the end of the text $s$ (after its last character). In one move, you can do one of the following actions:</p><ul> <li> press the "left" button, so the cursor is moved to the left by one position (or does nothing if it is pointing at the beginning of the text, i. e. before its first character); </li><li> press the "right" button, so the cursor is moved to the right by one position (or does nothing if it is pointing at the end of the text, i. e. after its last character); </li><li> press the "home" button, so the cursor is moved to the beginning of the text (before the first character of the text); </li><li> press the "end" button, so the cursor is moved to the end of the text (after the last character of the text); </li><li> press the "backspace" button, so the character before the cursor is removed from the text (if there is no such character, nothing happens). </li></ul><p>Your task is to calculate the minimum number of moves required to obtain the text $t$ from the text $s$ using the given set of actions, or determine it is impossible to obtain the text $t$ from the text $s$.</p><p>You have to answer $T$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $T$ ($1 \le T \le 5000$) — the number of test cases. Then $T$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $m$ ($1 \le m \le n \le 5000$) — the length of $s$ and the length of $t$, respectively.</p><p>The second line of the test case contains the string $s$ consisting of $n$ lowercase Latin letters.</p><p>The third line of the test case contains the string $t$ consisting of $m$ lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$ ($\sum n \le 5000$).</p></div><div class="output-specification"><p>For each test case, print one integer — the minimum number of moves required to obtain the text $t$ from the text $s$ using the given set of actions, or <span class="tex-font-style-tt">-1</span> if it is impossible to obtain the text $t$ from the text $s$ in the given test case.</p></div>

## Input

<p>The first line of the input contains one integer $T$ ($1 \le T \le 5000$) — the number of test cases. Then $T$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $m$ ($1 \le m \le n \le 5000$) — the length of $s$ and the length of $t$, respectively.</p><p>The second line of the test case contains the string $s$ consisting of $n$ lowercase Latin letters.</p><p>The third line of the test case contains the string $t$ consisting of $m$ lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$ ($\sum n \le 5000$).</p>

## Output

<p>For each test case, print one integer — the minimum number of moves required to obtain the text $t$ from the text $s$ using the given set of actions, or <span class="tex-font-style-tt">-1</span> if it is impossible to obtain the text $t$ from the text $s$ in the given test case.</p>





```input1|2,3,4,8,9,10,14,15,16
6
9 4
aaaaaaaaa
aaaa
7 3
abacaba
aaa
5 4
aabcd
abcd
4 2
abba
bb
6 4
baraka
baka
8 7
question
problem
```




```output1
5
6
3
4
4
-1
```


