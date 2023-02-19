## Description

<div><p>You are given a binary string $s$ consisting of $n$ zeros and ones.</p><p>Your task is to divide the given string into the <span class="tex-font-style-bf">minimum</span> number of <span class="tex-font-style-bf">subsequences</span> in such a way that <span class="tex-font-style-it">each character</span> of the string belongs to exactly <span class="tex-font-style-it">one subsequence</span> and each subsequence looks like "<span class="tex-font-style-tt">010101 ...</span>" or "<span class="tex-font-style-tt">101010 ...</span>" (i.e. the subsequence should not contain two adjacent zeros or ones).</p><p>Recall that a subsequence is a sequence that can be derived from the given sequence by deleting zero or more elements without changing the order of the remaining elements. For example, subsequences of "<span class="tex-font-style-tt">1011101</span>" are "<span class="tex-font-style-tt">0</span>", "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">11111</span>", "<span class="tex-font-style-tt">0111</span>", "<span class="tex-font-style-tt">101</span>", "<span class="tex-font-style-tt">1001</span>", but not "<span class="tex-font-style-tt">000</span>", "<span class="tex-font-style-tt">101010</span>" and "<span class="tex-font-style-tt">11100</span>".</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $s$. The second line of the test case contains $n$ characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' — the string $s$.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer: in the first line print one integer $k$ ($1 \le k \le n$) — the minimum number of subsequences you can divide the string $s$ to. In the second line print $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le k$), where $a_i$ is the number of subsequence the $i$-th character of $s$ belongs to.</p><p>If there are several answers, you can print any.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $s$. The second line of the test case contains $n$ characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' — the string $s$.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer: in the first line print one integer $k$ ($1 \le k \le n$) — the minimum number of subsequences you can divide the string $s$ to. In the second line print $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le k$), where $a_i$ is the number of subsequence the $i$-th character of $s$ belongs to.</p><p>If there are several answers, you can print any.</p>





```input1
4
4
0011
6
111111
5
10101
8
01010000
```




```output1
2
1 2 2 1 
6
1 2 3 4 5 6 
1
1 1 1 1 1 
4
1 1 1 1 1 2 3 4
```


