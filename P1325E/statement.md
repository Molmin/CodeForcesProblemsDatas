## Description

<div><p>You are given an array $a$ of length $n$ that has a special condition: every element in this array has at most 7 divisors. Find the length of the shortest non-empty subsequence of this array product of whose elements is a perfect square.</p><p>A sequence $a$ is a subsequence of an array $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) elements.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of $a$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($1 \le a_i \le 10^6$)&nbsp;— the elements of the array $a$.</p></div><div class="output-specification"><p>Output the length of the shortest non-empty subsequence of $a$ product of whose elements is a perfect square. If there are several shortest subsequences, you can find any of them. If there's no such subsequence, print "-1".</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of $a$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($1 \le a_i \le 10^6$)&nbsp;— the elements of the array $a$.</p>

## Output

<p>Output the length of the shortest non-empty subsequence of $a$ product of whose elements is a perfect square. If there are several shortest subsequences, you can find any of them. If there's no such subsequence, print "-1".</p>





```input1
3
1 4 6
```




```input2
4
2 3 6 6
```




```input3
3
6 15 10
```




```input4
4
2 3 5 7
```




```output1
1
```




```output2
2
```




```output3
3
```




```output4
-1
```



## Note

<p>In the first sample, you can choose a subsequence $[1]$.</p><p>In the second sample, you can choose a subsequence $[6, 6]$.</p><p>In the third sample, you can choose a subsequence $[6, 15, 10]$.</p><p>In the fourth sample, there is no such subsequence.</p>
