## Description

<div><p>Ehab loves number theory, but for some reason he hates the number $x$. Given an array $a$, find the length of its longest subarray such that the sum of its elements <span class="tex-font-style-bf">isn't</span> divisible by $x$, or determine that such subarray doesn't exist.</p><p>An array $a$ is a subarray of an array $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end.</p></div><div class="input-specification"><p>The first line contains an integer $t$ $(1 \le t \le 5)$&nbsp;— the number of test cases you need to solve. The description of the test cases follows.</p><p>The first line of each test case contains 2 integers $n$ and $x$ ($1 \le n \le 10^5$, $1 \le x \le 10^4$)&nbsp;— the number of elements in the array $a$ and the number that Ehab hates.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($0 \le a_i \le 10^4$)&nbsp;— the elements of the array $a$.</p></div><div class="output-specification"><p>For each testcase, print the length of the longest subarray whose sum isn't divisible by $x$. If there's no such subarray, print $-1$.</p></div>

## Input

<p>The first line contains an integer $t$ $(1 \le t \le 5)$&nbsp;— the number of test cases you need to solve. The description of the test cases follows.</p><p>The first line of each test case contains 2 integers $n$ and $x$ ($1 \le n \le 10^5$, $1 \le x \le 10^4$)&nbsp;— the number of elements in the array $a$ and the number that Ehab hates.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($0 \le a_i \le 10^4$)&nbsp;— the elements of the array $a$.</p>

## Output

<p>For each testcase, print the length of the longest subarray whose sum isn't divisible by $x$. If there's no such subarray, print $-1$.</p>





```input1
3
3 3
1 2 3
3 4
1 2 3
2 2
0 6
```




```output1
2
3
-1
```



## Note

<p>In the first test case, the subarray $[2,3]$ has sum of elements $5$, which isn't divisible by $3$.</p><p>In the second test case, the sum of elements of the whole array is $6$, which isn't divisible by $4$.</p><p>In the third test case, all subarrays have an even sum, so the answer is $-1$.</p>
