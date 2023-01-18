## Description

<div><p>Anu has created her own function $f$: $f(x, y) = (x | y) - y$ where $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>. For example, $f(11, 6) = (11|6) - 6 = 15 - 6 = 9$. It can be proved that for any nonnegative numbers $x$ and $y$ value of $f(x, y)$ is also nonnegative. </p><p>She would like to research more about this function and has created multiple problems for herself. But she isn't able to solve all of them and needs your help. Here is one of these problems.</p><p>A value of an array $[a_1, a_2, \dots, a_n]$ is defined as $f(f(\dots f(f(a_1, a_2), a_3), \dots a_{n-1}), a_n)$ (see notes). You are given an array with <span class="tex-font-style-bf">not necessarily distinct</span> elements. How should you reorder its elements so that the value of the array is maximal possible?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$). Elements of the array are <span class="tex-font-style-bf">not guaranteed</span> to be different.</p></div><div class="output-specification"><p>Output $n$ integers, the reordering of the array with maximum value. If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$). Elements of the array are <span class="tex-font-style-bf">not guaranteed</span> to be different.</p>

## Output

<p>Output $n$ integers, the reordering of the array with maximum value. If there are multiple answers, print any.</p>





```input1
4
4 0 11 6
```




```input2
1
13
```




```output1
11 6 4 0
```




```output2
13
```



## Note

<p>In the first testcase, value of the array $[11, 6, 4, 0]$ is $f(f(f(11, 6), 4), 0) = f(f(9, 4), 0) = f(9, 0) = 9$.</p><p>$[11, 4, 0, 6]$ is also a valid answer.</p>
