## Description

<div><p>Given an array $a$ of length $n$, find another array, $b$, of length $n$ such that:</p><ul> <li> for each $i$ $(1 \le i \le n)$ $MEX(\{b_1$, $b_2$, $\ldots$, $b_i\})=a_i$. </li></ul><p>The $MEX$ of a set of integers is the smallest non-negative integer that doesn't belong to this set.</p><p>If such array doesn't exist, determine this.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, $\ldots$, $a_n$ ($0 \le a_i \le i$)&nbsp;— the elements of the array $a$. <span class="tex-font-style-bf">It's guaranteed that $a_i \le a_{i+1}$ for $1\le i &lt; n$.</span> </p></div><div class="output-specification"><p>If there's no such array, print a single line containing $-1$.</p><p>Otherwise, print a single line containing $n$ integers $b_1$, $b_2$, $\ldots$, $b_n$ ($0 \le b_i \le 10^6$)</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, $\ldots$, $a_n$ ($0 \le a_i \le i$)&nbsp;— the elements of the array $a$. <span class="tex-font-style-bf">It's guaranteed that $a_i \le a_{i+1}$ for $1\le i &lt; n$.</span> </p>

## Output

<p>If there's no such array, print a single line containing $-1$.</p><p>Otherwise, print a single line containing $n$ integers $b_1$, $b_2$, $\ldots$, $b_n$ ($0 \le b_i \le 10^6$)</p><p>If there are multiple answers, print any.</p>





```input1
3
1 2 3
```




```input2
4
0 0 0 2
```




```input3
3
1 1 3
```




```output1
0 1 2
```




```output2
1 3 4 0
```




```output3
0 2 1
```



## Note

<p>In the second test case, other answers like $[1,1,1,0]$, for example, are valid.</p>
