## Description

<div><p>Some programming website is establishing a secure communication protocol. For security reasons, they want to choose several more or less random strings.</p><p>Initially, they have a string $s$ consisting of lowercase English letters. Now they want to choose $q$ strings using the following steps, and you are to help them.</p><ol> <li> A string $x$ consisting of lowercase English letters and integers $l$ and $r$ ($1 \leq l \leq r \leq |s|$) are chosen. </li><li> Consider all non-empty distinct substrings of the $s_l s_{l + 1} \ldots s_r$, that is all distinct strings $s_i s_{i+1} \ldots s_{j}$ where $l \le i \le j \le r$. Among all of them choose all strings that are lexicographically greater than $x$. </li><li> If there are no such strings, you should print $-1$. Otherwise print the lexicographically smallest among them. </li></ol><p>String $a$ is lexicographically less than string $b$, if either $a$ is a prefix of $b$ and $a \ne b$, or there exists such a position $i$ ($1 \le i \le min(|a|, |b|)$), such that $a_i &lt; b_i$ and for all $j$ ($1 \le j &lt; i$) $a_j = b_j$. Here $|a|$ denotes the length of the string $a$.</p></div><div class="input-specification"><p>The first line of input contains a non-empty string $s$ ($1 \leq |s| \leq 10^{5}$) consisting of lowercase English letters.</p><p>The second line contains an integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of strings to select.</p><p>Each of the next $q$ lines contains two integers $l$, $r$ ($1 \leq l \leq r \leq |s|$) and a non-empty string $x$ consisting of lowercase English letters. The total length of strings $x$ for all queries does not exceed $2 \cdot 10^{5}$.</p></div><div class="output-specification"><p>Output $q$ lines, each of them should contain the desired string or $-1$, if there is no such string.</p></div>

## Input

<p>The first line of input contains a non-empty string $s$ ($1 \leq |s| \leq 10^{5}$) consisting of lowercase English letters.</p><p>The second line contains an integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of strings to select.</p><p>Each of the next $q$ lines contains two integers $l$, $r$ ($1 \leq l \leq r \leq |s|$) and a non-empty string $x$ consisting of lowercase English letters. The total length of strings $x$ for all queries does not exceed $2 \cdot 10^{5}$.</p>

## Output

<p>Output $q$ lines, each of them should contain the desired string or $-1$, if there is no such string.</p>





```input1
baa
5
1 2 ba
2 3 a
1 2 b
2 3 aa
1 3 b

```




```input2
bacb
4
1 2 ba
2 3 ac
1 3 ac
3 4 c

```




```input3
bba
1
1 1 b

```




```output1
-1
aa
ba
-1
ba

```




```output2
-1
c
b
cb

```




```output3
-1

```



## Note

<p>Consider the first example.</p><p>The string $s$ is "<span class="tex-font-style-tt">baa</span>". The queries are as follows.</p><ol> <li> We consider the substring $s_1 s_2$ that is "<span class="tex-font-style-tt">ba</span>". It has substrings "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">ba</span>", since none of them is greater than the query string "<span class="tex-font-style-tt">ba</span>", the answer is $-1$.</li><li> We consider substring "<span class="tex-font-style-tt">aa</span>". Among its substrings only "<span class="tex-font-style-tt">aa</span>" is greater than the query string "<span class="tex-font-style-tt">a</span>". So the answer is "<span class="tex-font-style-tt">aa</span>".</li><li> We consider substring "<span class="tex-font-style-tt">ba</span>". Out of "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">ba</span>" only "<span class="tex-font-style-tt">ba</span>" is greater than the query string "<span class="tex-font-style-tt">b</span>", so the answer is "<span class="tex-font-style-tt">ba</span>".</li><li> We consider substring "<span class="tex-font-style-tt">aa</span>". No substring of "<span class="tex-font-style-tt">aa</span>" is greater than the query string "<span class="tex-font-style-tt">aa</span>" so the answer is $-1$.</li><li> We consider substring "<span class="tex-font-style-tt">baa</span>" and it has (among others) substrings "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">baa</span>" which are greater than the query string "<span class="tex-font-style-tt">b</span>". Since "<span class="tex-font-style-tt">ba</span>" is lexicographically smaller than "<span class="tex-font-style-tt">baa</span>", the answer is "<span class="tex-font-style-tt">ba</span>". </li></ol>
