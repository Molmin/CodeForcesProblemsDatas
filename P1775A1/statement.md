## Description

<div><p><span class="tex-font-style-bf">This is an easy version of the problem. The difference between the versions is that the string can be longer than in the easy version. You can only do hacks if both versions of the problem are passed.</span></p><p>Kazimir Kazimirovich is a Martian gardener. He has a huge orchard of binary balanced apple trees.</p><p>Recently Casimir decided to get himself three capybaras. The gardener even came up with their names and wrote them down on a piece of paper. The name of each capybara is a non-empty line consisting of letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>".</p><p>Denote the names of the capybaras by the lines $a$, $b$, and $c$. Then Casimir wrote the nonempty lines $a$, $b$, and $c$ in a row without spaces. For example, if the capybara's name was "<span class="tex-font-style-tt">aba</span>", "<span class="tex-font-style-tt">ab</span>", and "<span class="tex-font-style-tt">bb</span>", then the string the gardener wrote down would look like "<span class="tex-font-style-tt">abaabbb</span>".</p><p>The gardener remembered an interesting property: either the string $b$ is lexicographically not smaller than the strings $a$ and $c$ at the same time, or the string $b$ is lexicographically not greater than the strings $a$ and $c$ at the same time. In other words, either $a \le b$ and $c \le b$ are satisfied, or $b \le a$ and $b \le c$ are satisfied (or possibly both conditions simultaneously). Here $\le$ denotes the lexicographic "less than or equal to" for strings. Thus, $a \le b$ means that the strings must either be equal, or the string $a$ must stand earlier in the dictionary than the string $b$. For a more detailed explanation of this operation, see "Notes" section.</p><p>Today the gardener looked at his notes and realized that he cannot recover the names because they are written without spaces. He is no longer sure if he can recover the original strings $a$, $b$, and $c$, so he wants to find any triplet of names that satisfy the above property.</p><center> <img class="tex-graphics" src="file://SuigBNSe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>The only line of a test case contains the string $s$ ($3 \le |s| \le 100$)&nbsp;— the names of the capybaras, written together. The string consists of English letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' only.</p><p>It is guaranteed that the sum of string lengths over all test cases does not exceed $500$.</p></div><div class="output-specification"><p>For each test case, print three strings $a$, $b$ and $c$ on a single line, separated by spaces&nbsp;— names of capybaras, such that writing them without spaces results in a line $s$. Either $a \le b$ and $c \le b$, or $b \le a$ and $b \le c$ must be satisfied.</p><p>If there are several ways to restore the names, print any of them. If the names cannot be recovered, print "<span class="tex-font-style-tt">:(</span>" (without quotes).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>The only line of a test case contains the string $s$ ($3 \le |s| \le 100$)&nbsp;— the names of the capybaras, written together. The string consists of English letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>' only.</p><p>It is guaranteed that the sum of string lengths over all test cases does not exceed $500$.</p>

## Output

<p>For each test case, print three strings $a$, $b$ and $c$ on a single line, separated by spaces&nbsp;— names of capybaras, such that writing them without spaces results in a line $s$. Either $a \le b$ and $c \le b$, or $b \le a$ and $b \le c$ must be satisfied.</p><p>If there are several ways to restore the names, print any of them. If the names cannot be recovered, print "<span class="tex-font-style-tt">:(</span>" (without quotes).</p>





```input1|2,4,6
5
bbba
aba
aaa
abba
abbb
```




```output1
b bb a
a b a
a a a
ab b a
a bb b
```



## Note

<p>A string $x$ is lexicographically smaller than a string $y$ if and only if one of the following holds: </p><ul> <li> $x$ is a prefix of $y$, but $x \ne y$; </li><li> in the first position where $x$ and $y$ differ, the string $x$ has the letter '<span class="tex-font-style-tt">a</span>', and the string $y$ has the letter '<span class="tex-font-style-tt">b</span>'. </li></ul><p>Now let's move on to the examples.</p><p>In the first test case, one of the possible ways to split the line $s$ into three lines&nbsp;— "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">bb</span>", "<span class="tex-font-style-tt">a</span>".</p><p>In the third test case, we can see that the split satisfies two conditions at once (i.&nbsp;e., $a \le b$, $c \le b$, $b \le a$, and $b \le c$ are true simultaneously).</p>
