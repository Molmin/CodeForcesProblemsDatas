## Description

<div><p>You are given a string $s$ of <span class="tex-font-style-tt">0</span>'s and <span class="tex-font-style-tt">1</span>'s. You are allowed to perform the following operation:</p><ul><li> choose a non-empty contiguous substring of $s$ that contains an equal number of <span class="tex-font-style-tt">0</span>'s and <span class="tex-font-style-tt">1</span>'s;</li><li> flip all characters in the substring, that is, replace all <span class="tex-font-style-tt">0</span>'s with <span class="tex-font-style-tt">1</span>'s, and vice versa;</li><li> reverse the substring. </li></ul><p>For example, consider $s$ = <span class="tex-font-style-tt">00111011</span>, and the following operation:</p><ul><li> Choose the first six characters as the substring to act upon: <span class="tex-font-style-tt"><span class="tex-font-style-bf">001110</span>11</span>. Note that the number of <span class="tex-font-style-tt">0</span>'s and <span class="tex-font-style-tt">1</span>'s are equal, so this is a legal choice. Choosing substrings <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">110</span>, or the entire string would not be possible.</li><li> Flip all characters in the substring: <span class="tex-font-style-tt"><span class="tex-font-style-bf">110001</span>11</span>.</li><li> Reverse the substring: <span class="tex-font-style-tt"><span class="tex-font-style-bf">100011</span>11</span>. </li></ul> <p>Find the lexicographically smallest string that can be obtained from $s$ after zero or more operations.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \leq T \leq 5 \cdot 10^5$)&nbsp;— the number of test cases. Each of the following $T$ lines contains a single non-empty string&nbsp;— the input string $s$ for the respective test case.</p><p>All strings consist of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>, and their total length does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, on a separate line print the lexicographically smallest string that can be obtained from $s$ after zero or more operations.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \leq T \leq 5 \cdot 10^5$)&nbsp;— the number of test cases. Each of the following $T$ lines contains a single non-empty string&nbsp;— the input string $s$ for the respective test case.</p><p>All strings consist of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>, and their total length does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, on a separate line print the lexicographically smallest string that can be obtained from $s$ after zero or more operations.</p>





```input1
3
100101
1100011
10101010
```




```output1
010110
0110110
10101010
```



## Note

<p>In the first test case a single operation should be applied to the entire string.</p><p>In the second test case two operations are needed: <span class="tex-font-style-tt"><span class="tex-font-style-bf">011100</span>1</span>, <span class="tex-font-style-tt">011<span class="tex-font-style-bf">0110</span></span>.</p><p>In the third test case the string stays the same after any operation.</p>
