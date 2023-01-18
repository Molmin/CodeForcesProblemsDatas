## Description

<div><p>You are given a string $s$ consisting only of lowercase Latin letters.</p><p>You can rearrange all letters of this string as you wish. Your task is to obtain a <span class="tex-font-style-bf">good</span> string by rearranging the letters of the given string or report that it is impossible to do it.</p><p>Let's call a string <span class="tex-font-style-bf">good</span> if it is not a palindrome. Palindrome is a string which is read from left to right the same as from right to left. For example, strings "<span class="tex-font-style-tt">abacaba</span>", "<span class="tex-font-style-tt">aa</span>" and "<span class="tex-font-style-tt">z</span>" are palindromes and strings "<span class="tex-font-style-tt">bba</span>", "<span class="tex-font-style-tt">xd</span>" are not.</p><p>You have to answer $t$ <span class="tex-font-style-bf">independent</span> queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — number of queries.</p><p>Each of the next $t$ lines contains one string. The $i$-th line contains a string $s_i$ consisting only of lowercase Latin letter. It is guaranteed that the <span class="tex-font-style-bf">length</span> of $s_i$ is <span class="tex-font-style-bf">from $1$ to $1000$</span> (inclusive).</p></div><div class="output-specification"><p>Print $t$ lines. In the $i$-th line print the answer to the $i$-th query: <span class="tex-font-style-tt">-1</span> if it is impossible to obtain a <span class="tex-font-style-bf">good</span> string by rearranging the letters of $s_i$ and <span class="tex-font-style-bf">any good</span> string which can be obtained from the given one (by rearranging the letters) otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — number of queries.</p><p>Each of the next $t$ lines contains one string. The $i$-th line contains a string $s_i$ consisting only of lowercase Latin letter. It is guaranteed that the <span class="tex-font-style-bf">length</span> of $s_i$ is <span class="tex-font-style-bf">from $1$ to $1000$</span> (inclusive).</p>

## Output

<p>Print $t$ lines. In the $i$-th line print the answer to the $i$-th query: <span class="tex-font-style-tt">-1</span> if it is impossible to obtain a <span class="tex-font-style-bf">good</span> string by rearranging the letters of $s_i$ and <span class="tex-font-style-bf">any good</span> string which can be obtained from the given one (by rearranging the letters) otherwise.</p>





```input1
3
aa
abacaba
xdd
```




```output1
-1
abaacba
xdd
```



## Note

<p>In the first query we cannot rearrange letters to obtain a <span class="tex-font-style-bf">good</span> string.</p><p>Other examples (not all) of correct answers to the second query: "<span class="tex-font-style-tt">ababaca</span>", "<span class="tex-font-style-tt">abcabaa</span>", "<span class="tex-font-style-tt">baacaba</span>".</p><p>In the third query we can do nothing to obtain a <span class="tex-font-style-bf">good</span> string.</p>
