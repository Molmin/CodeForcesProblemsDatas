## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between the versions is in the constraints on the array elements. You can make hacks only if all versions of the problem are solved.</span></p><p>You are given an array $[a_1, a_2, \dots, a_n]$. </p><p>Your goal is to find the length of the longest subarray of this array such that the most frequent value in it is <span class="tex-font-style-bf">not</span> unique. In other words, you are looking for a subarray such that if the most frequent value occurs $f$ times in this subarray, then at least $2$ different values should occur exactly $f$ times.</p><p>An array $c$ is a subarray of an array $d$ if $c$ can be obtained from $d$ by deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 200\,000$)&nbsp;— the length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le min(n, 100)$)&nbsp;— elements of the array.</p></div><div class="output-specification"><p>You should output exactly one integer &nbsp;— the length of the longest subarray of the array whose most frequent value is not unique. If there is no such subarray, output $0$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 200\,000$)&nbsp;— the length of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le min(n, 100)$)&nbsp;— elements of the array.</p>

## Output

<p>You should output exactly one integer &nbsp;— the length of the longest subarray of the array whose most frequent value is not unique. If there is no such subarray, output $0$.</p>





```input1
7
1 1 2 2 3 3 3
```




```input2
10
1 1 1 5 4 1 3 1 2 2
```




```input3
1
1
```




```output1
6
```




```output2
7
```




```output3
0
```



## Note

<p>In the first sample, the subarray $[1, 1, 2, 2, 3, 3]$ is good, but $[1, 1, 2, 2, 3, 3, 3]$ isn't: in the latter there are $3$ occurrences of number $3$, and no other element appears $3$ times.</p>
