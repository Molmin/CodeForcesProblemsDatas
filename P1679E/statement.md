## Description

<div><p><span class="tex-font-style-it">Today is a holiday in the residence hall&nbsp;— Oleh arrived, in honor of which the girls gave him a string. Oleh liked the gift a lot, so he immediately thought up and offered you, his best friend, the following problem.</span></p><p>You are given a string $s$ of length $n$, which consists of the first $17$ lowercase Latin letters {$a$, $b$, $c$, $\ldots$, $p$, $q$} and question marks. And $q$ queries. Each query is defined by a set of pairwise distinct lowercase first $17$ letters of the Latin alphabet, which can be used to replace the question marks in the string $s$.</p><p>The answer to the query is the sum of the number of distinct substrings that are palindromes over all strings that can be obtained from the original string $s$ by replacing question marks with available characters. The answer must be calculated modulo $998\,244\,353$.</p><p><span class="tex-font-style-bf">Pay attention!</span> Two substrings are different when their start and end positions in the string are different. So, the number of different substrings that are palindromes for the string <span class="tex-font-style-tt">aba</span> will be $4$: <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">aba</span>.</p><p>Consider examples of replacing question marks with letters. For example, from the string <span class="tex-font-style-tt">aba??ee</span> when querying {$a$, $b$} you can get the strings <span class="tex-font-style-tt">ababaee</span> or <span class="tex-font-style-tt">abaaaee</span> but you cannot get the strings <span class="tex-font-style-tt">pizza</span>, <span class="tex-font-style-tt"> abaee</span>, <span class="tex-font-style-tt">abacaba</span>, <span class="tex-font-style-tt">aba?fee</span>, <span class="tex-font-style-tt">aba47ee</span>, or <span class="tex-font-style-tt">abatree</span>.</p><p>Recall that a palindrome is a string that reads the same from left to right as from right to left.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 1\,000$)&nbsp;— the length of the string $s$.</p><p>The second line contains the string $s$, which consists of $n$ lowercase Latin letters and question marks. It is guaranteed that all letters in the string belong to the set {$a$, $b$, $c$, $\ldots$, $p$, $q$}.</p><p>The third line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>This is followed by $q$ lines, each containing a single line $t$&nbsp;— a set of characters that can replace question marks ($1 \le |t| \le 17$). It is guaranteed that all letters in the string belong to the set {$a$, $b$, $c$, $\ldots$, $p$, $q$} and occur at most once.</p></div><div class="output-specification"><p>For each query print one number&nbsp;— the total numbers of palindromic substrings in all strings that can be obtained from the string $s$, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 1\,000$)&nbsp;— the length of the string $s$.</p><p>The second line contains the string $s$, which consists of $n$ lowercase Latin letters and question marks. It is guaranteed that all letters in the string belong to the set {$a$, $b$, $c$, $\ldots$, $p$, $q$}.</p><p>The third line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>This is followed by $q$ lines, each containing a single line $t$&nbsp;— a set of characters that can replace question marks ($1 \le |t| \le 17$). It is guaranteed that all letters in the string belong to the set {$a$, $b$, $c$, $\ldots$, $p$, $q$} and occur at most once.</p>

## Output

<p>For each query print one number&nbsp;— the total numbers of palindromic substrings in all strings that can be obtained from the string $s$, modulo $998\,244\,353$.</p>





```input1
7
ab??aba
8
a
b
ab
abc
abcd
abcde
abcdef
abcdefg
```




```input2
11
???????????
6
abcdefghijklmnopq
ecpnkhbmlidgfjao
olehfan
codef
glhf
q
```




```output1
14
13
55
105
171
253
351
465
```




```output2
900057460
712815817
839861037
756843750
70840320
66
```



## Note

<p>Consider the first example and the first query in it. We can get only one string as a result of replacing the question marks &nbsp;— <span class="tex-font-style-tt">abaaaba</span>. It has the following palindrome substrings: </p><ol> <li> <span class="tex-font-style-tt">a</span> &nbsp;— substring [$1$; $1$]. </li><li> <span class="tex-font-style-tt">b</span> &nbsp;— substring [$2$; $2$]. </li><li> <span class="tex-font-style-tt">a</span> &nbsp;— substring [$3$; $3$]. </li><li> <span class="tex-font-style-tt">a</span> &nbsp;— substring [$4$; $4$]. </li><li> <span class="tex-font-style-tt">a</span> &nbsp;— substring [$5$; $5$]. </li><li> <span class="tex-font-style-tt">b</span> &nbsp;— substring [$6$; $6$]. </li><li> <span class="tex-font-style-tt">a</span> &nbsp;— substring [$7$; $7$]. </li><li> <span class="tex-font-style-tt">aa</span> &nbsp;— substring [$3$; $4$]. </li><li> <span class="tex-font-style-tt">aa</span> &nbsp;— substring [$4$; $5$]. </li><li> <span class="tex-font-style-tt">aba</span> &nbsp;— substring [$1$; $3$]. </li><li> <span class="tex-font-style-tt">aaa</span> &nbsp;— substring [$3$; $5$]. </li><li> <span class="tex-font-style-tt">aba</span> &nbsp;— substring [$5$; $7$]. </li><li> <span class="tex-font-style-tt">baaab</span> &nbsp;— substring [$2$; $6$]. </li><li> <span class="tex-font-style-tt">abaaaba</span> &nbsp;— substring [$1$; $7$]. </li></ol><p>In the third request, we get 4 lines: <span class="tex-font-style-tt">abaaaba</span>, <span class="tex-font-style-tt">abababa</span>, <span class="tex-font-style-tt">abbaaba</span>, <span class="tex-font-style-tt">abbbaba</span>.</p>
