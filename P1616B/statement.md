## Description

<div><p>You have a string $s_1 s_2 \ldots s_n$ and you stand on the left of the string looking right. You want to choose an index $k$ ($1 \le k \le n$) and place a mirror after the $k$-th letter, so that what you see is $s_1 s_2 \ldots s_k s_k s_{k - 1} \ldots s_1$. What is the lexicographically smallest string you can see?</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds: </p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul></div><div class="input-specification"><p>The first line of input contains one integer $t$ ($1 \leq t \leq 10\,000$): the number of test cases.</p><p>The next $t$ lines contain the description of the test cases, two lines per a test case.</p><p>In the first line you are given one integer $n$ ($1 \leq n \leq 10^5$): the length of the string.</p><p>The second line contains the string $s$ consisting of $n$ lowercase English characters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print the lexicographically smallest string you can see.</p></div>

## Input

<p>The first line of input contains one integer $t$ ($1 \leq t \leq 10\,000$): the number of test cases.</p><p>The next $t$ lines contain the description of the test cases, two lines per a test case.</p><p>In the first line you are given one integer $n$ ($1 \leq n \leq 10^5$): the length of the string.</p><p>The second line contains the string $s$ consisting of $n$ lowercase English characters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print the lexicographically smallest string you can see.</p>





```input1
4
10
codeforces
9
cbacbacba
3
aaa
4
bbaa
```




```output1
cc
cbaabc
aa
bb
```



## Note

<p>In the first test case choose $k = 1$ to obtain "<span class="tex-font-style-tt">cc</span>".</p><p>In the second test case choose $k = 3$ to obtain "<span class="tex-font-style-tt">cbaabc</span>".</p><p>In the third test case choose $k = 1$ to obtain "<span class="tex-font-style-tt">aa</span>".</p><p>In the fourth test case choose $k = 1$ to obtain "<span class="tex-font-style-tt">bb</span>".</p>
