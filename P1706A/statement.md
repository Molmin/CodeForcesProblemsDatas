## Description

<div><p>You have a sequence $a_1, a_2, \ldots, a_n$ of length $n$, consisting of integers between $1$ and $m$. You also have a string $s$, consisting of $m$ characters <span class="tex-font-style-tt">B</span>.</p><p>You are going to perform the following $n$ operations. </p><ul> <li> At the $i$-th ($1 \le i \le n$) operation, you replace either the $a_i$-th <span class="tex-font-style-bf">or</span> the $(m + 1 - a_i)$-th character of $s$ with <span class="tex-font-style-tt">A</span>. You can replace the character at any position multiple times through the operations. </li></ul><p>Find the lexicographically smallest string you can get after these operations.</p><p>A string $x$ is lexicographically smaller than a string $y$ of the same length if and only if in the first position where $x$ and $y$ differ, the string $x$ has a letter that appears earlier in the alphabet than the corresponding letter in $y$.</p></div><div class="input-specification"><p>The first line contains the number of test cases $t$ ($1 \le t \le 2000$).</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 50$)&nbsp;— the length of the sequence $a$ and the length of the string $s$ respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le m$)&nbsp;— the sequence $a$.</p></div><div class="output-specification"><p>For each test case, print a string of length $m$&nbsp;— the lexicographically smallest string you can get. Each character of the string should be either capital English letter <span class="tex-font-style-tt">A</span> or capital English letter <span class="tex-font-style-tt">B</span>.</p></div>

## Input

<p>The first line contains the number of test cases $t$ ($1 \le t \le 2000$).</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 50$)&nbsp;— the length of the sequence $a$ and the length of the string $s$ respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le m$)&nbsp;— the sequence $a$.</p>

## Output

<p>For each test case, print a string of length $m$&nbsp;— the lexicographically smallest string you can get. Each character of the string should be either capital English letter <span class="tex-font-style-tt">A</span> or capital English letter <span class="tex-font-style-tt">B</span>.</p>





```input1|2,3,6,7,10,11
6
4 5
1 1 3 1
1 5
2
4 1
1 1 1 1
2 4
1 3
2 7
7 5
4 5
5 5 3 5
```




```output1
ABABA
BABBB
A
AABB
ABABBBB
ABABA
```



## Note

<p>In the first test case, the sequence $a = [1, 1, 3, 1]$. One of the possible solutions is the following. </p><ul> <li> At the $1$-st operation, you can replace the $1$-st character of $s$ with <span class="tex-font-style-tt">A</span>. After it, $s$ becomes <span class="tex-font-style-tt"><span class="tex-font-style-underline">A</span>BBBB</span>. </li><li> At the $2$-nd operation, you can replace the $5$-th character of $s$ with <span class="tex-font-style-tt">A</span> (since $m+1-a_2=5$). After it, $s$ becomes <span class="tex-font-style-tt">ABBB<span class="tex-font-style-underline">A</span></span>. </li><li> At the $3$-rd operation, you can replace the $3$-rd character of $s$ with <span class="tex-font-style-tt">A</span>. After it, $s$ becomes <span class="tex-font-style-tt">AB<span class="tex-font-style-underline">A</span>BA</span>. </li><li> At the $4$-th operation, you can replace the $1$-st character of $s$ with <span class="tex-font-style-tt">A</span>. After it, $s$ remains equal to <span class="tex-font-style-tt">ABABA</span>. </li></ul> The resulting string is <span class="tex-font-style-tt">ABABA</span>. It is impossible to produce a lexicographically smaller string.<p>In the second test case, you are going to perform only one operation. You can replace either the $2$-nd character or $4$-th character of $s$ with <span class="tex-font-style-tt">A</span>. You can get strings <span class="tex-font-style-tt">BABBB</span> and <span class="tex-font-style-tt">BBBAB</span> after the operation. The string <span class="tex-font-style-tt">BABBB</span> is the lexicographically smallest among these strings.</p><p>In the third test case, the only string you can get is <span class="tex-font-style-tt">A</span>.</p><p>In the fourth test case, you can replace the $1$-st and $2$-nd characters of $s$ with <span class="tex-font-style-tt">A</span> to get <span class="tex-font-style-tt">AABB</span>.</p><p>In the fifth test case, you can replace the $1$-st and $3$-rd characters of $s$ with <span class="tex-font-style-tt">A</span> to get <span class="tex-font-style-tt">ABABBBB</span>.</p>
