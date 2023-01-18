## Description

<div><p>At Moscow Workshops ICPC team gets a balloon for each problem they solved first. Team MSU Red Panda got so many balloons that they didn't know how to spend them. So they came up with a problem with them.</p><p>There are several balloons, not more than $10^6$ in total, each one is colored in one of $k$ colors. We can perform the following operation: choose $k-1$ balloons such that they are of $k-1$ different colors, and recolor them all into remaining color. We can perform this operation any finite number of times (for example, we can only perform the operation if there are at least $k-1$ different colors among current balls).</p><p>How many different balloon configurations can we get? Only number of balloons of each color matters, configurations differing only by the order of balloons are counted as equal. As this number can be very large, output it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains a single integer $k$ ($2 \le k \le 10^5$)&nbsp;—the number of colors.</p><p>The second line contains $k$ integers $a_1, a_2, \ldots, a_k$ ($0 \le a_i$)&nbsp;—initial configuration of balloons. $a_i$ is number of balloons of color $i$. The total number of balloons doesn't exceed $10^6$. In other words,</p><p>$a_1 + a_2 + a_3 + \ldots + a_k \le 10^6$.</p></div><div class="output-specification"><p>Output number of possible configurations modulo $998244353$.</p></div>

## Input

<p>The first line contains a single integer $k$ ($2 \le k \le 10^5$)&nbsp;—the number of colors.</p><p>The second line contains $k$ integers $a_1, a_2, \ldots, a_k$ ($0 \le a_i$)&nbsp;—initial configuration of balloons. $a_i$ is number of balloons of color $i$. The total number of balloons doesn't exceed $10^6$. In other words,</p><p>$a_1 + a_2 + a_3 + \ldots + a_k \le 10^6$.</p>

## Output

<p>Output number of possible configurations modulo $998244353$.</p>





```input1
3
0 1 2
```




```input2
4
1 1 1 1
```




```input3
5
0 0 1 2 3
```




```input4
3
2 2 8
```




```output1
3
```




```output2
5
```




```output3
1
```




```output4
31
```



## Note

<p>In the first example, there are $3$ configurations we can get: $[0, 1, 2]$, $[2, 0, 1]$, $[1, 2, 0]$.</p><p>In the second example, we can apply the operation not more than once, and possible configurations are: $[1, 1, 1, 1]$, $[0, 0, 0, 4]$, $[0, 0, 4, 0]$, $[0, 4, 0, 0]$, $[4, 0, 0, 0]$. </p><p>In the third example, we can't apply any operations, so the only achievable configuration is the starting one.</p>
