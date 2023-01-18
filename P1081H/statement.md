## Description

<div><p>After learning some fancy algorithms about palindromes, Chouti found palindromes very interesting, so he wants to challenge you with this problem.</p><p>Chouti has got two strings $A$ and $B$. Since he likes <a href="https://en.wikipedia.org/wiki/Palindrome">palindromes</a>, he would like to pick $a$ as some non-empty palindromic substring of $A$ and $b$ as some non-empty palindromic substring of $B$. Concatenating them, he will get string $ab$.</p><p>Chouti thinks strings he could get this way are interesting, so he wants to know how many different strings he can get.</p></div><div class="input-specification"><p>The first line contains a single string $A$ ($1 \le |A| \le 2 \cdot 10^5$).</p><p>The second line contains a single string $B$ ($1 \le |B| \le 2 \cdot 10^5$).</p><p>Strings $A$ and $B$ contain only lowercase English letters.</p></div><div class="output-specification"><p>The first and only line should contain a single integer&nbsp;— the number of possible strings.</p></div>

## Input

<p>The first line contains a single string $A$ ($1 \le |A| \le 2 \cdot 10^5$).</p><p>The second line contains a single string $B$ ($1 \le |B| \le 2 \cdot 10^5$).</p><p>Strings $A$ and $B$ contain only lowercase English letters.</p>

## Output

<p>The first and only line should contain a single integer&nbsp;— the number of possible strings.</p>





```input1
aa
aba

```




```input2
aaba
abaa

```




```output1
6

```




```output2
15

```



## Note

<p>In the first example, attainable strings are </p><ul> <li> "<span class="tex-font-style-tt">a</span>" + "<span class="tex-font-style-tt">a</span>" = "aa", </li><li> "<span class="tex-font-style-tt">aa</span>" + "<span class="tex-font-style-tt">a</span>" = "<span class="tex-font-style-tt">aaa</span>", </li><li> "<span class="tex-font-style-tt">aa</span>" + "<span class="tex-font-style-tt">aba</span>" = "<span class="tex-font-style-tt">aaaba</span>", </li><li> "<span class="tex-font-style-tt">aa</span>" + "<span class="tex-font-style-tt">b</span>" = "<span class="tex-font-style-tt">aab</span>", </li><li> "<span class="tex-font-style-tt">a</span>" + "<span class="tex-font-style-tt">aba</span>" = "<span class="tex-font-style-tt">aaba</span>", </li><li> "<span class="tex-font-style-tt">a</span>" + "<span class="tex-font-style-tt">b</span>" = "<span class="tex-font-style-tt">ab</span>". </li></ul><p>In the second example, attainable strings are "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">aaaa</span>", "<span class="tex-font-style-tt">aaaba</span>", "<span class="tex-font-style-tt">aab</span>", "<span class="tex-font-style-tt">aaba</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">abaa</span>", "<span class="tex-font-style-tt">abaaa</span>", "<span class="tex-font-style-tt">abaaba</span>", "<span class="tex-font-style-tt">abab</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">baa</span>", "<span class="tex-font-style-tt">baba</span>", "<span class="tex-font-style-tt">bb</span>".</p><p>Notice that though "<span class="tex-font-style-tt">a</span>"+"<span class="tex-font-style-tt">aa</span>"="<span class="tex-font-style-tt">aa</span>"+"<span class="tex-font-style-tt">a</span>"="<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">aaa</span>" will only be counted once.</p>
