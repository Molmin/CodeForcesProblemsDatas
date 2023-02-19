## Description

<div><p>XYMXYM and CQXYM will prepare $n$ problems for Codeforces. The difficulty of the problem $i$ will be an integer $a_i$, where $a_i \geq 0$. The difficulty of the problems must satisfy $a_i+a_{i+1}&lt;m$ ($1 \leq i &lt; n$), and $a_1+a_n&lt;m$, where $m$ is a fixed integer. XYMXYM wants to know how many plans of the difficulty of the problems there are modulo $998\,244\,353$.</p><p>Two plans of difficulty $a$ and $b$ are different only if there is an integer $i$ ($1 \leq i \leq n$) satisfying $a_i \neq b_i$.</p></div><div class="input-specification"><p>A single line contains two integers $n$ and $m$ ($2 \leq n \leq 50\,000$, $1 \leq m \leq 10^9$).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of different plans.</p></div>

## Input

<p>A single line contains two integers $n$ and $m$ ($2 \leq n \leq 50\,000$, $1 \leq m \leq 10^9$).</p>

## Output

<p>Print a single integer&nbsp;— the number of different plans.</p>





```input1
3 2
```




```input2
5 9
```




```input3
21038 3942834
```




```output1
4
```




```output2
8105
```




```output3
338529212
```



## Note

<p>In the first test case, the valid $a$ are: $[0,0,0]$, $[0,0,1]$, $[0,1,0]$, $[1,0,0]$.</p><p>$[1,0,1]$ is invalid since $a_1+a_n \geq m$.</p>
