## Description

<div><p>You are given a string $s$ consisting of $n$ lowercase Latin letters. $n$ is even.</p><p>For each position $i$ ($1 \le i \le n$) in string $s$ you are required to change the letter on this position either to the previous letter in alphabetic order or to the next one (letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">z</span>' have only one of these options). Letter in every position must be changed <span class="tex-font-style-bf">exactly once</span>.</p><p>For example, letter '<span class="tex-font-style-tt">p</span>' should be changed either to '<span class="tex-font-style-tt">o</span>' or to '<span class="tex-font-style-tt">q</span>', letter '<span class="tex-font-style-tt">a</span>' should be changed to '<span class="tex-font-style-tt">b</span>' and letter '<span class="tex-font-style-tt">z</span>' should be changed to '<span class="tex-font-style-tt">y</span>'.</p><p>That way string "<span class="tex-font-style-tt">codeforces</span>", for example, can be changed to "<span class="tex-font-style-tt">dpedepqbft</span>" ('<span class="tex-font-style-tt">c</span>' $\rightarrow$ '<span class="tex-font-style-tt">d</span>', '<span class="tex-font-style-tt">o</span>' $\rightarrow$ '<span class="tex-font-style-tt">p</span>', '<span class="tex-font-style-tt">d</span>' $\rightarrow$ '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">e</span>' $\rightarrow$ '<span class="tex-font-style-tt">d</span>', '<span class="tex-font-style-tt">f</span>' $\rightarrow$ '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">o</span>' $\rightarrow$ '<span class="tex-font-style-tt">p</span>', '<span class="tex-font-style-tt">r</span>' $\rightarrow$ '<span class="tex-font-style-tt">q</span>', '<span class="tex-font-style-tt">c</span>' $\rightarrow$ '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">e</span>' $\rightarrow$ '<span class="tex-font-style-tt">f</span>', '<span class="tex-font-style-tt">s</span>' $\rightarrow$ '<span class="tex-font-style-tt">t</span>').</p><p>String $s$ is called a palindrome if it reads the same from left to right and from right to left. For example, strings "<span class="tex-font-style-tt">abba</span>" and "<span class="tex-font-style-tt">zz</span>" are palindromes and strings "<span class="tex-font-style-tt">abca</span>" and "<span class="tex-font-style-tt">zy</span>" are not.</p><p>Your goal is to check if it's possible to make string $s$ a palindrome by applying the aforementioned changes to every position. Print "<span class="tex-font-style-tt">YES</span>" if string $s$ can be transformed to a palindrome and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>Each testcase contains several strings, for each of them you are required to solve the problem separately.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 50$) — the number of strings in a testcase.</p><p>Then $2T$ lines follow — lines $(2i - 1)$ and $2i$ of them describe the $i$-th string. The first line of the pair contains a single integer $n$ ($2 \le n \le 100$, $n$ is even) — the length of the corresponding string. The second line of the pair contains a string $s$, consisting of $n$ lowercase Latin letters.</p></div><div class="output-specification"><p>Print $T$ lines. The $i$-th line should contain the answer to the $i$-th string of the input. Print "<span class="tex-font-style-tt">YES</span>" if it's possible to make the $i$-th string a palindrome by applying the aforementioned changes to every position. Print "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 50$) — the number of strings in a testcase.</p><p>Then $2T$ lines follow — lines $(2i - 1)$ and $2i$ of them describe the $i$-th string. The first line of the pair contains a single integer $n$ ($2 \le n \le 100$, $n$ is even) — the length of the corresponding string. The second line of the pair contains a string $s$, consisting of $n$ lowercase Latin letters.</p>

## Output

<p>Print $T$ lines. The $i$-th line should contain the answer to the $i$-th string of the input. Print "<span class="tex-font-style-tt">YES</span>" if it's possible to make the $i$-th string a palindrome by applying the aforementioned changes to every position. Print "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
5
6
abccba
2
cf
4
adfa
8
abaazaba
2
ml

```




```output1
YES
NO
YES
NO
NO

```



## Note

<p>The first string of the example can be changed to "<span class="tex-font-style-tt">bcbbcb</span>", two leftmost letters and two rightmost letters got changed to the next letters, two middle letters got changed to the previous letters.</p><p>The second string can be changed to "<span class="tex-font-style-tt">be</span>", "<span class="tex-font-style-tt">bg</span>", "<span class="tex-font-style-tt">de</span>", "<span class="tex-font-style-tt">dg</span>", but none of these resulting strings are palindromes.</p><p>The third string can be changed to "<span class="tex-font-style-tt">beeb</span>" which is a palindrome.</p><p>The fifth string can be changed to "<span class="tex-font-style-tt">lk</span>", "<span class="tex-font-style-tt">lm</span>", "<span class="tex-font-style-tt">nk</span>", "<span class="tex-font-style-tt">nm</span>", but none of these resulting strings are palindromes. Also note that no letter can remain the same, so you can't obtain strings "<span class="tex-font-style-tt">ll</span>" or "<span class="tex-font-style-tt">mm</span>".</p>
