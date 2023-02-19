## Description

<div><p>You are given a string $s$ consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p><p>You have to remove several (possibly zero) characters from the beginning of the string, and then several (possibly zero) characters from the end of the string. <span class="tex-font-style-bf">The string may become empty after the removals</span>. The cost of the removal is the <span class="tex-font-style-bf">maximum</span> of the following two values:</p><ul> <li> the number of characters <span class="tex-font-style-tt">0</span> left in the string; </li><li> the number of characters <span class="tex-font-style-tt">1</span> removed from the string. </li></ul><p>What is the <span class="tex-font-style-bf">minimum</span> cost of removal you can achieve?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of one line containing the string $s$ ($1 \le |s| \le 2 \cdot 10^5$), consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p><p>The total length of strings $s$ in all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer — the minimum cost of removal you can achieve.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of one line containing the string $s$ ($1 \le |s| \le 2 \cdot 10^5$), consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p><p>The total length of strings $s$ in all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer — the minimum cost of removal you can achieve.</p>





```input1
5
101110110
1001001001001
0000111111
00000
1111
```




```output1
1
3
0
0
0
```



## Note

<p>Consider the test cases of the example:</p><ol> <li> in the first test case, it's possible to remove two characters from the beginning and one character from the end. Only one <span class="tex-font-style-tt">1</span> is deleted, only one <span class="tex-font-style-tt">0</span> remains, so the cost is $1$; </li><li> in the second test case, it's possible to remove three characters from the beginning and six characters from the end. Two characters <span class="tex-font-style-tt">0</span> remain, three characters <span class="tex-font-style-tt">1</span> are deleted, so the cost is $3$; </li><li> in the third test case, it's optimal to remove four characters from the beginning; </li><li> in the fourth test case, it's optimal to remove the whole string; </li><li> in the fifth test case, it's optimal to leave the string as it is. </li></ol>
