## Description

<div><p>Given the integer $n$&nbsp;— the number of available blocks. You must use <span class="tex-font-style-bf">all</span> blocks to build a <span class="tex-font-style-it">pedestal</span>. </p><p>The <span class="tex-font-style-it">pedestal</span> consists of $3$ platforms for $2$-nd, $1$-st and $3$-rd places respectively. The platform for the $1$-st place must be <span class="tex-font-style-bf">strictly</span> higher than for the $2$-nd place, and the platform for the $2$-nd place must be <span class="tex-font-style-bf">strictly</span> higher than for the $3$-rd place. Also, the height of each platform must be greater than zero (that is, each platform must contain at least one block).</p><center> <img class="tex-graphics" src="file://GtZGiAng.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Example pedestal of $n=11$ blocks: second place height equals $4$ blocks, first place height equals $5$ blocks, third place height equals $2$ blocks.</span></center><p>Among all possible pedestals of $n$ blocks, deduce one such that the platform height for the $1$-st place <span class="tex-font-style-bf">minimum</span> as possible. If there are several of them, output any of them.</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case contains a single integer $n$ ($6 \le n \le 10^5$)&nbsp;— the total number of blocks for the pedestal. All $n$ blocks must be used.</p><p>It is guaranteed that the sum of $n$ values over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output $3$ numbers $h_2, h_1, h_3$&nbsp;— the platform heights for $2$-nd, $1$-st and $3$-rd places on a pedestal consisting of $n$ blocks ($h_1+h_2+h_3=n$, $0 &lt; h_3 &lt; h_2 &lt; h_1$). </p><p>Among all possible pedestals, output the one for which the value of $h_1$ <span class="tex-font-style-bf">minimal</span>. If there are several of them, output any of them.</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case contains a single integer $n$ ($6 \le n \le 10^5$)&nbsp;— the total number of blocks for the pedestal. All $n$ blocks must be used.</p><p>It is guaranteed that the sum of $n$ values over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output $3$ numbers $h_2, h_1, h_3$&nbsp;— the platform heights for $2$-nd, $1$-st and $3$-rd places on a pedestal consisting of $n$ blocks ($h_1+h_2+h_3=n$, $0 &lt; h_3 &lt; h_2 &lt; h_1$). </p><p>Among all possible pedestals, output the one for which the value of $h_1$ <span class="tex-font-style-bf">minimal</span>. If there are several of them, output any of them.</p>





```input1
6
11
6
10
100000
7
8
```




```output1
4 5 2
2 3 1
4 5 1
33334 33335 33331
2 4 1
3 4 1
```



## Note

<p>In the first test case we can not get the height of the platform for the first place less than $5$, because if the height of the platform for the first place is not more than $4$, then we can use at most $4 + 3 + 2 = 9$ blocks. And we should use $11 = 4 + 5 + 2$ blocks. Therefore, the answer <span class="tex-font-style-tt">4 5 2</span> fits. </p><p>In the second set, the only suitable answer is: <span class="tex-font-style-tt">2 3 1</span>.</p>
