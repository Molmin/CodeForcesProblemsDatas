## Description

<div><p>You are given a string $s$, consisting only of characters '0' and '1'.</p><p>You have to choose a contiguous substring of $s$ and remove all occurrences of the character, which is a strict minority in it, from the substring.</p><p>That is, if the amount of '0's in the substring is strictly smaller than the amount of '1's, remove all occurrences of '0' from the substring. If the amount of '1's is strictly smaller than the amount of '0's, remove all occurrences of '1'. If the amounts are the same, do nothing.</p><p>You have to apply the operation <span class="tex-font-style-bf">exactly once</span>. What is the maximum amount of characters that can be removed?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains a non-empty string $s$, consisting only of characters '0' and '1'. The length of $s$ doesn't exceed $2 \cdot 10^5$.</p><p>The total length of strings $s$ over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— the maximum amount of characters that can be removed after applying the operation <span class="tex-font-style-bf">exactly once</span>.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains a non-empty string $s$, consisting only of characters '0' and '1'. The length of $s$ doesn't exceed $2 \cdot 10^5$.</p><p>The total length of strings $s$ over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print a single integer&nbsp;— the maximum amount of characters that can be removed after applying the operation <span class="tex-font-style-bf">exactly once</span>.</p>





```input1
4
01
1010101010111
00110001000
1
```




```output1
0
5
3
0
```



## Note

<p>In the first testcase, you can choose substrings "0", "1" or "01". In "0" the amount of '0' is $1$, the amount of '1' is $0$. '1' is a strict minority, thus all occurrences of it are removed from the substring. However, since there were $0$ of them, nothing changes. Same for "1". And in "01" neither of '0' or '1' is a strict minority. Thus, nothing changes. So there is no way to remove any characters.</p><p>In the second testcase, you can choose substring "10101010101". It contains $5$ characters '0' and $6$ characters '1'. '0' is a strict minority. Thus, you can remove all its occurrences. There exist other substrings that produce the same answer.</p><p>In the third testcase, you can choose substring "011000100". It contains $6$ characters '0' and $3$ characters '1'. '1' is a strict minority. Thus, you can remove all its occurrences.</p>
