## Description

<div><p>You are given a string $s$ of length $n$. Each character is either one of the first $k$ lowercase Latin letters or a question mark.</p><p>You are asked to replace every question mark with one of the first $k$ lowercase Latin letters in such a way that the following value is maximized.</p><p>Let $f_i$ be the maximum length substring of string $s$, which consists entirely of the $i$-th Latin letter. A substring of a string is a contiguous subsequence of that string. If the $i$-th letter doesn't appear in a string, then $f_i$ is equal to $0$.</p><p>The value of a string $s$ is the minimum value among $f_i$ for all $i$ from $1$ to $k$.</p><p>What is the maximum value the string can have?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$; $1 \le k \le 17$)&nbsp;— the length of the string and the number of first Latin letters used.</p><p>The second line contains a string $s$, consisting of $n$ characters. Each character is either one of the first $k$ lowercase Latin letters or a question mark.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum value of the string after every question mark is replaced with one of the first $k$ lowercase Latin letters.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$; $1 \le k \le 17$)&nbsp;— the length of the string and the number of first Latin letters used.</p><p>The second line contains a string $s$, consisting of $n$ characters. Each character is either one of the first $k$ lowercase Latin letters or a question mark.</p>

## Output

<p>Print a single integer&nbsp;— the maximum value of the string after every question mark is replaced with one of the first $k$ lowercase Latin letters.</p>





```input1
10 2
a??ab????b
```




```input2
9 4
?????????
```




```input3
2 3
??
```




```input4
15 3
??b?babbc??b?aa
```




```input5
4 4
cabd
```




```output1
4
```




```output2
2
```




```output3
0
```




```output4
3
```




```output5
1
```



## Note

<p>In the first example the question marks can be replaced in the following way: "<span class="tex-font-style-tt">a<span class="tex-font-style-underline">aa</span>ab<span class="tex-font-style-underline">abbb</span>b</span>". $f_1 = 4$, $f_2 = 4$, thus the answer is $4$. Replacing it like this is also possible: "<span class="tex-font-style-tt">a<span class="tex-font-style-underline">aa</span>ab<span class="tex-font-style-underline">bbbb</span>b</span>". That way $f_1 = 4$, $f_2 = 6$, however, the minimum of them is still $4$.</p><p>In the second example one of the possible strings is "<span class="tex-font-style-tt"><span class="tex-font-style-underline">aabbccdda</span></span>".</p><p>In the third example at least one letter won't appear in the string, thus, the minimum of values $f_i$ is always $0$.</p>
