## Description

<div><p>A non-empty digit string is <span class="tex-font-style-it">diverse</span> if the number of occurrences of each character in it doesn't exceed the number of distinct characters in it.</p><p>For example: </p><ul> <li> string "<span class="tex-font-style-tt">7</span>" is diverse because <span class="tex-font-style-tt">7</span> appears in it $1$ time and the number of distinct characters in it is $1$; </li><li> string "<span class="tex-font-style-tt">77</span>" is <span class="tex-font-style-bf">not</span> diverse because <span class="tex-font-style-tt">7</span> appears in it $2$ times and the number of distinct characters in it is $1$; </li><li> string "<span class="tex-font-style-tt">1010</span>" is diverse because both <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span> appear in it $2$ times and the number of distinct characters in it is $2$; </li><li> string "<span class="tex-font-style-tt">6668</span>" is <span class="tex-font-style-bf">not</span> diverse because <span class="tex-font-style-tt">6</span> appears in it $3$ times and the number of distinct characters in it is $2$. </li></ul><p>You are given a string $s$ of length $n$, consisting of only digits $0$ to $9$. Find how many of its $\frac{n(n+1)}{2}$ substrings are diverse.</p><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p><p>Note that if the same diverse string appears in $s$ multiple times, each occurrence should be counted independently. For example, there are two diverse substrings in "<span class="tex-font-style-tt">77</span>" both equal to "<span class="tex-font-style-tt">7</span>", so the answer for the string "<span class="tex-font-style-tt">77</span>" is $2$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$. It is guaranteed that all characters of $s$ are digits from $0$ to $9$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print one integer&nbsp;— the number of diverse substrings of the given string $s$. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$. It is guaranteed that all characters of $s$ are digits from $0$ to $9$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print one integer&nbsp;— the number of diverse substrings of the given string $s$. </p>





```input1|2,3,6,7,10,11,14,15
7
1
7
2
77
4
1010
5
01100
6
399996
5
23456
18
789987887987998798
```




```output1
1
2
10
12
10
15
106
```



## Note

<p>In the first test case, the diverse substring is "<span class="tex-font-style-tt">7</span>".</p><p>In the second test case, the only diverse substring is "<span class="tex-font-style-tt">7</span>", which appears twice, so the answer is $2$.</p><p>In the third test case, the diverse substrings are "<span class="tex-font-style-tt">0</span>" ($2$ times), "<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">010</span>", "<span class="tex-font-style-tt">1</span>" ($2$ times), "<span class="tex-font-style-tt">10</span>" ($2$ times), "<span class="tex-font-style-tt">101</span>" and "<span class="tex-font-style-tt">1010</span>".</p><p>In the fourth test case, the diverse substrings are "<span class="tex-font-style-tt">0</span>" ($3$ times), "<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">011</span>", "<span class="tex-font-style-tt">0110</span>", "<span class="tex-font-style-tt">1</span>" ($2$ times), "<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">100</span>", "<span class="tex-font-style-tt">110</span>" and "<span class="tex-font-style-tt">1100</span>".</p><p>In the fifth test case, the diverse substrings are "<span class="tex-font-style-tt">3</span>", "<span class="tex-font-style-tt">39</span>", "<span class="tex-font-style-tt">399</span>", "<span class="tex-font-style-tt">6</span>", "<span class="tex-font-style-tt">9</span>" ($4$ times), "<span class="tex-font-style-tt">96</span>" and "<span class="tex-font-style-tt">996</span>".</p><p>In the sixth test case, all $15$ non-empty substrings of "<span class="tex-font-style-tt">23456</span>" are diverse.</p>
