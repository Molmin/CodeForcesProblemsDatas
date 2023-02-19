## Description

<div><p>Let's call the string <span class="tex-font-style-bf">beautiful</span> if it does not contain a substring of length at least $2$, which is a palindrome. Recall that a palindrome is a string that reads the same way from the first character to the last and from the last character to the first. For example, the strings <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">bab</span>, <span class="tex-font-style-tt">acca</span>, <span class="tex-font-style-tt">bcabcbacb</span> are palindromes, but the strings <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">abbbaa</span>, <span class="tex-font-style-tt">cccb</span> are not.</p><p>Let's define <span class="tex-font-style-bf">cost</span> of a string as the minimum number of operations so that the string becomes beautiful, if in one operation it is allowed to change any character of the string to one of the first $3$ letters of the Latin alphabet (in lowercase).</p><p>You are given a string $s$ of length $n$, each character of the string is one of the first $3$ letters of the Latin alphabet (in lowercase).</p><p>You have to answer $m$ queries&nbsp;— calculate the cost of the substring of the string $s$ from $l_i$-th to $r_i$-th position, inclusive.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$)&nbsp;— the length of the string $s$ and the number of queries.</p><p>The second line contains the string $s$, it consists of $n$ characters, each character one of the first $3$ Latin letters.</p><p>The following $m$ lines contain two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— parameters of the $i$-th query.</p></div><div class="output-specification"><p>For each query, print a single integer&nbsp;— the cost of the substring of the string $s$ from $l_i$-th to $r_i$-th position, inclusive.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$)&nbsp;— the length of the string $s$ and the number of queries.</p><p>The second line contains the string $s$, it consists of $n$ characters, each character one of the first $3$ Latin letters.</p><p>The following $m$ lines contain two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— parameters of the $i$-th query.</p>

## Output

<p>For each query, print a single integer&nbsp;— the cost of the substring of the string $s$ from $l_i$-th to $r_i$-th position, inclusive.</p>





```input1
5 4
baacb
1 3
1 5
4 5
2 3
```




```output1
1
2
0
1
```



## Note

<p>Consider the queries of the example test.</p><ul> <li> in the first query, the substring is <span class="tex-font-style-tt">baa</span>, which can be changed to <span class="tex-font-style-tt">bac</span> in one operation; </li><li> in the second query, the substring is <span class="tex-font-style-tt">baacb</span>, which can be changed to <span class="tex-font-style-tt">cbacb</span> in two operations; </li><li> in the third query, the substring is <span class="tex-font-style-tt">cb</span>, which can be left unchanged; </li><li> in the fourth query, the substring is <span class="tex-font-style-tt">aa</span>, which can be changed to <span class="tex-font-style-tt">ba</span> in one operation. </li></ul>
