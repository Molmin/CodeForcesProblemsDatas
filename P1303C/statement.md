## Description

<div><p>Polycarp wants to assemble his own keyboard. Layouts with multiple rows are too complicated for him — his keyboard will consist of only one row, where all $26$ lowercase Latin letters will be arranged in some order.</p><p>Polycarp uses the same password $s$ on all websites where he is registered (it is bad, but he doesn't care). He wants to assemble a keyboard that will allow to type this password very easily. He doesn't like to move his fingers while typing the password, so, for each pair of adjacent characters in $s$, they should be adjacent on the keyboard. For example, if the password is <span class="tex-font-style-tt">abacaba</span>, then the layout <span class="tex-font-style-tt">cabdefghi...</span> is perfect, since characters <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">c</span> are adjacent on the keyboard, and <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span> are adjacent on the keyboard. It is guaranteed that there are no two adjacent equal characters in $s$, so, for example, the password cannot be <span class="tex-font-style-tt">password</span> (two characters <span class="tex-font-style-tt">s</span> are adjacent).</p><p>Can you help Polycarp with choosing the perfect layout of the keyboard, if it is possible?</p></div><div class="input-specification"><p>The first line contains one integer $T$ ($1 \le T \le 1000$) — the number of test cases.</p><p>Then $T$ lines follow, each containing one string $s$ ($1 \le |s| \le 200$) representing the test case. $s$ consists of lowercase Latin letters only. There are no two adjacent equal characters in $s$.</p></div><div class="output-specification"><p>For each test case, do the following:</p><ul> <li> if it is impossible to assemble a perfect keyboard, print <span class="tex-font-style-tt">NO</span> (in upper case, <span class="tex-font-style-bf">it matters in this problem</span>); </li><li> otherwise, print <span class="tex-font-style-tt">YES</span> (in upper case), and then a string consisting of $26$ lowercase Latin letters — the perfect layout. Each Latin letter should appear in this string exactly once. If there are multiple answers, print any of them. </li></ul></div>

## Input

<p>The first line contains one integer $T$ ($1 \le T \le 1000$) — the number of test cases.</p><p>Then $T$ lines follow, each containing one string $s$ ($1 \le |s| \le 200$) representing the test case. $s$ consists of lowercase Latin letters only. There are no two adjacent equal characters in $s$.</p>

## Output

<p>For each test case, do the following:</p><ul> <li> if it is impossible to assemble a perfect keyboard, print <span class="tex-font-style-tt">NO</span> (in upper case, <span class="tex-font-style-bf">it matters in this problem</span>); </li><li> otherwise, print <span class="tex-font-style-tt">YES</span> (in upper case), and then a string consisting of $26$ lowercase Latin letters — the perfect layout. Each Latin letter should appear in this string exactly once. If there are multiple answers, print any of them. </li></ul>





```input1
5
ababa
codedoca
abcda
zxzytyz
abcdefghijklmnopqrstuvwxyza
```




```output1
YES
bacdefghijklmnopqrstuvwxyz
YES
edocabfghijklmnpqrstuvwxyz
NO
YES
xzytabcdefghijklmnopqrsuvw
NO
```


