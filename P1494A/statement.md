## Description

<div><p>You are given a string $a$, consisting of $n$ characters, $n$ is even. For each $i$ from $1$ to $n$ $a_i$ is one of '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">C</span>'.</p><p>A bracket sequence is a string containing only characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>". A regular bracket sequence is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">+</span>" between the original characters of the sequence. For example, bracket sequences "<span class="tex-font-style-tt">()()</span>" and "<span class="tex-font-style-tt">(())</span>" are regular (the resulting expressions are: "<span class="tex-font-style-tt">(1)+(1)</span>" and "<span class="tex-font-style-tt">((1+1)+1)</span>"), and "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" are not.</p><p>You want to find a string $b$ that consists of $n$ characters such that: </p><ul> <li> $b$ is a regular bracket sequence; </li><li> if for some $i$ and $j$ ($1 \le i, j \le n$) $a_i=a_j$, then $b_i=b_j$. </li></ul><p>In other words, you want to replace all occurrences of '<span class="tex-font-style-tt">A</span>' with the same type of bracket, then all occurrences of '<span class="tex-font-style-tt">B</span>' with the same type of bracket and all occurrences of '<span class="tex-font-style-tt">C</span>' with the same type of bracket.</p><p>Your task is to determine if such a string $b$ exists.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The only line of each testcase contains a string $a$. $a$ consists only of uppercase letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>' and '<span class="tex-font-style-tt">C</span>'. Let $n$ be the length of $a$. It is guaranteed that $n$ is even and $2 \le n \le 50$.</p></div><div class="output-specification"><p>For each testcase print "<span class="tex-font-style-tt">YES</span>" if there exists such a string $b$ that: </p><ul> <li> $b$ is a regular bracket sequence; </li><li> if for some $i$ and $j$ ($1 \le i, j \le n$) $a_i=a_j$, then $b_i=b_j$. </li></ul><p>Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The only line of each testcase contains a string $a$. $a$ consists only of uppercase letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>' and '<span class="tex-font-style-tt">C</span>'. Let $n$ be the length of $a$. It is guaranteed that $n$ is even and $2 \le n \le 50$.</p>

## Output

<p>For each testcase print "<span class="tex-font-style-tt">YES</span>" if there exists such a string $b$ that: </p><ul> <li> $b$ is a regular bracket sequence; </li><li> if for some $i$ and $j$ ($1 \le i, j \le n$) $a_i=a_j$, then $b_i=b_j$. </li></ul><p>Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p>





```input1
4
AABBAC
CACA
BBBBAC
ABCA
```




```output1
YES
YES
NO
NO
```



## Note

<p>In the first testcase one of the possible strings $b$ is "<span class="tex-font-style-tt">(())()</span>".</p><p>In the second testcase one of the possible strings $b$ is "<span class="tex-font-style-tt">()()</span>".</p>
