## Description

<div><p>Polycarp has a string $s$. Polycarp performs the following actions until the string $s$ is empty ($t$ is initially an empty string):</p><ul> <li> he adds to the right to the string $t$ the string $s$, i.e. he does $t = t + s$, where $t + s$ is a concatenation of the strings $t$ and $s$; </li><li> he selects an arbitrary letter of $s$ and removes from $s$ all its occurrences (<span class="tex-font-style-bf">the selected letter must occur in the string $s$ at the moment of performing this action</span>). </li></ul><p>Polycarp performs this sequence of actions <span class="tex-font-style-bf">strictly</span> in this order.</p><p>Note that after Polycarp finishes the actions, the string $s$ will be empty and the string $t$ will be equal to some value (that is undefined and depends on the order of removing).</p><p>E.g. consider $s$="<span class="tex-font-style-tt">abacaba</span>" so the actions may be performed as follows:</p><ul> <li> $t$="<span class="tex-font-style-tt">abacaba</span>", the letter '<span class="tex-font-style-tt">b</span>' is selected, then $s$="<span class="tex-font-style-tt">aacaa</span>"; </li><li> $t$="<span class="tex-font-style-tt">abacabaaacaa</span>", the letter '<span class="tex-font-style-tt">a</span>' is selected, then $s$="<span class="tex-font-style-tt">c</span>"; </li><li> $t$="<span class="tex-font-style-tt">abacabaaacaac</span>", the letter '<span class="tex-font-style-tt">c</span>' is selected, then $s$="" (the empty string). </li></ul><p>You need to restore the initial value of the string $s$ using only the final value of $t$ and find the order of removing letters from $s$.</p></div><div class="input-specification"><p>The first line contains one integer $T$ ($1 \le T \le 10^4$) — the number of test cases. Then $T$ test cases follow.</p><p>Each test case contains one string $t$ consisting of lowercase letters of the Latin alphabet. The length of $t$ doesn't exceed $5 \cdot 10^5$. The sum of lengths of all strings $t$ in the test cases doesn't exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output in a separate line:</p><ul> <li> $-1$, if the answer doesn't exist; </li><li> two strings separated by spaces. The first one must contain a possible initial value of $s$. The second one must contain a sequence of letters — it's in what order one needs to remove letters from $s$ to make the string $t$. E.g. if the string "<span class="tex-font-style-tt">bac</span>" is outputted, then, first, all occurrences of the letter '<span class="tex-font-style-tt">b</span>' were deleted, then all occurrences of '<span class="tex-font-style-tt">a</span>', and then, finally, all occurrences of '<span class="tex-font-style-tt">c</span>'. If there are multiple solutions, print any one. </li></ul></div>

## Input

<p>The first line contains one integer $T$ ($1 \le T \le 10^4$) — the number of test cases. Then $T$ test cases follow.</p><p>Each test case contains one string $t$ consisting of lowercase letters of the Latin alphabet. The length of $t$ doesn't exceed $5 \cdot 10^5$. The sum of lengths of all strings $t$ in the test cases doesn't exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case output in a separate line:</p><ul> <li> $-1$, if the answer doesn't exist; </li><li> two strings separated by spaces. The first one must contain a possible initial value of $s$. The second one must contain a sequence of letters — it's in what order one needs to remove letters from $s$ to make the string $t$. E.g. if the string "<span class="tex-font-style-tt">bac</span>" is outputted, then, first, all occurrences of the letter '<span class="tex-font-style-tt">b</span>' were deleted, then all occurrences of '<span class="tex-font-style-tt">a</span>', and then, finally, all occurrences of '<span class="tex-font-style-tt">c</span>'. If there are multiple solutions, print any one. </li></ul>





```input1
7
abacabaaacaac
nowyouknowthat
polycarppoycarppoyarppyarppyrpprppp
isi
everywherevrywhrvryhrvrhrvhv
haaha
qweqeewew
```




```output1
abacaba bac
-1
polycarp lcoayrp
is si
everywhere ewyrhv
-1
-1
```



## Note

<p>The first test case is considered in the statement.</p>
