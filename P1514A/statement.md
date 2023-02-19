## Description

<div><p>Given an array $a$ of length $n$, tell us whether it has a non-empty subsequence such that the product of its elements is <span class="tex-font-style-bf">not</span> a perfect square.</p><p>A sequence $b$ is a subsequence of an array $a$ if $b$ can be obtained from $a$ by deleting some (possibly zero) elements.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($1 \le a_i \le 10^4$)&nbsp;— the elements of the array $a$.</p></div><div class="output-specification"><p>If there's a subsequence of $a$ whose product isn't a perfect square, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($1 \le a_i \le 10^4$)&nbsp;— the elements of the array $a$.</p>

## Output

<p>If there's a subsequence of $a$ whose product isn't a perfect square, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
2
3
1 5 4
2
100 10000
```




```output1
YES
NO
```



## Note

<p>In the first example, the product of the whole array ($20$) isn't a perfect square.</p><p>In the second example, all subsequences have a perfect square product.</p>
