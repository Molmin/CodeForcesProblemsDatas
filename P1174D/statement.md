## Description

<div><p>Given two integers $n$ and $x$, construct an array that satisfies the following conditions: </p><ul> <li> for any element $a_i$ in the array, $1 \le a_i&lt;2^n$; </li><li> there is no <span class="tex-font-style-bf">non-empty</span> subsegment with <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> equal to $0$ or $x$, </li><li> its length $l$ should be maximized. </li></ul><p>A sequence $b$ is a subsegment of a sequence $a$ if $b$ can be obtained from $a$ by deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $x$ ($1 \le n \le 18$, $1 \le x&lt;2^{18}$).</p></div><div class="output-specification"><p>The first line should contain the length of the array $l$.</p><p>If $l$ is positive, the second line should contain $l$ space-separated integers $a_1$, $a_2$, $\dots$, $a_l$ ($1 \le a_i &lt; 2^n$)&nbsp;— the elements of the array $a$.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The only line contains two integers $n$ and $x$ ($1 \le n \le 18$, $1 \le x&lt;2^{18}$).</p>

## Output

<p>The first line should contain the length of the array $l$.</p><p>If $l$ is positive, the second line should contain $l$ space-separated integers $a_1$, $a_2$, $\dots$, $a_l$ ($1 \le a_i &lt; 2^n$)&nbsp;— the elements of the array $a$.</p><p>If there are multiple solutions, print any of them.</p>





```input1
3 5
```




```input2
2 4
```




```input3
1 1
```




```output1
3
6 1 3
```




```output2
3
1 3 1
```




```output3
0
```



## Note

<p>In the first example, the bitwise XOR of the subsegments are $\{6,7,4,1,2,3\}$.</p>
