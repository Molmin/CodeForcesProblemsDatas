## Description

<div><p>You are given two integers $l$ and $r$.</p><p>Let's call an integer $x$ <span class="tex-font-style-it">modest</span>, if $l \le x \le r$.</p><p>Find a string of length $n$, consisting of digits, which has the largest possible number of substrings, which make a modest integer. Substring having leading zeros are not counted. If there are many answers, find lexicographically smallest one.</p><p>If some number occurs multiple times as a substring, then in the counting of the number of modest substrings it is counted multiple times as well.</p></div><div class="input-specification"><p>The first line contains one integer $l$ ($1 \le l \le 10^{800}$).</p><p>The second line contains one integer $r$ ($l \le r \le 10^{800}$).</p><p>The third line contains one integer $n$ ($1 \le n \le 2\,000$).</p></div><div class="output-specification"><p>In the first line, print the maximum possible number of modest substrings.</p><p>In the second line, print a string of length $n$ having exactly that number of modest substrings.</p><p>If there are multiple such strings, print the lexicographically smallest of them.</p></div>

## Input

<p>The first line contains one integer $l$ ($1 \le l \le 10^{800}$).</p><p>The second line contains one integer $r$ ($l \le r \le 10^{800}$).</p><p>The third line contains one integer $n$ ($1 \le n \le 2\,000$).</p>

## Output

<p>In the first line, print the maximum possible number of modest substrings.</p><p>In the second line, print a string of length $n$ having exactly that number of modest substrings.</p><p>If there are multiple such strings, print the lexicographically smallest of them.</p>





```input1
1
10
3
```




```input2
1
11
3
```




```input3
12345
12346
6
```




```output1
3
101
```




```output2
5
111
```




```output3
1
012345
```



## Note

<p>In the first example, string «<span class="tex-font-style-tt">101</span>» has modest substrings «<span class="tex-font-style-tt">1</span>», «<span class="tex-font-style-tt">10</span>», «<span class="tex-font-style-tt">1</span>».</p><p>In the second example, string «<span class="tex-font-style-tt">111</span>» has modest substrings «<span class="tex-font-style-tt">1</span>» ($3$ times) and «<span class="tex-font-style-tt">11</span>» ($2$ times).</p>
