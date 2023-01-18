## Description

<div><p>You are given a binary string of length $n$ (i. e. a string consisting of $n$ characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>').</p><p>In one move you can swap two adjacent characters of the string. What is the lexicographically minimum possible string you can obtain from the given one if you can perform <span class="tex-font-style-bf">no more</span> than $k$ moves? It is possible that you do not perform any moves at all.</p><p>Note that you can swap the same pair of adjacent characters with indices $i$ and $i+1$ arbitrary (possibly, zero) number of times. Each such swap is considered a separate move.</p><p>You have to answer $q$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 10^4$) — the number of test cases.</p><p>The first line of the test case contains two integers $n$ and $k$ ($1 \le n \le 10^6, 1 \le k \le n^2$) — the length of the string and the number of moves you can perform.</p><p>The second line of the test case contains one string consisting of $n$ characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$ ($\sum n \le 10^6$).</p></div><div class="output-specification"><p>For each test case, print the answer on it: the lexicographically minimum possible string of length $n$ you can obtain from the given one if you can perform <span class="tex-font-style-bf">no more</span> than $k$ moves.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 10^4$) — the number of test cases.</p><p>The first line of the test case contains two integers $n$ and $k$ ($1 \le n \le 10^6, 1 \le k \le n^2$) — the length of the string and the number of moves you can perform.</p><p>The second line of the test case contains one string consisting of $n$ characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$ ($\sum n \le 10^6$).</p>

## Output

<p>For each test case, print the answer on it: the lexicographically minimum possible string of length $n$ you can obtain from the given one if you can perform <span class="tex-font-style-bf">no more</span> than $k$ moves.</p>





```input1
3
8 5
11011010
7 9
1111100
7 11
1111100
```




```output1
01011110
0101111
0011111
```



## Note

<p>In the first example, you can change the string as follows: $1\underline{10}11010 \rightarrow \underline{10}111010 \rightarrow 0111\underline{10}10 \rightarrow 011\underline{10}110 \rightarrow 01\underline{10}1110 \rightarrow 01011110$. </p><p>In the third example, there are enough operations to make the string sorted.</p>
