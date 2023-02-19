## Description

<div><p>There are $n$ people in a horizontal line, each looking either to the left or the right. Each person counts the number of people in the direction they are looking. The <span class="tex-font-style-bf">value</span> of the line is the sum of each person's count.</p><p>For example, in the arrangement <span class="tex-font-style-tt">LRRLL</span>, where <span class="tex-font-style-tt">L</span> stands for a person looking left and <span class="tex-font-style-tt">R</span> stands for a person looking right, the counts for each person are $[0, 3, 2, 3, 4]$, and the value is $0+3+2+3+4=12$.</p><p>You are given the initial arrangement of people in the line. For each $k$ from $1$ to $n$, determine the maximum value of the line if you can change the direction of <span class="tex-font-style-bf">at most</span> $k$ people.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the line.</p><p>The following line contains a string consisting of $n$ characters, each of which is either <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">R</span>, representing a person facing left or right, respectively&nbsp;— the description of the line.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p><p>Please note that the answer for some test cases won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p></div><div class="output-specification"><p>For each test case, output $n$ space-separated non-negative integers&nbsp;— the maximum value of the line if you can change the direction of <span class="tex-font-style-bf">at most</span> $k$ people for each $k$ from $1$ to $n$, inclusive.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the line.</p><p>The following line contains a string consisting of $n$ characters, each of which is either <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">R</span>, representing a person facing left or right, respectively&nbsp;— the description of the line.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p><p>Please note that the answer for some test cases won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p>

## Output

<p>For each test case, output $n$ space-separated non-negative integers&nbsp;— the maximum value of the line if you can change the direction of <span class="tex-font-style-bf">at most</span> $k$ people for each $k$ from $1$ to $n$, inclusive.</p>





```input1|2,3,6,7,10,11
6
3
LLR
5
LRRLL
1
L
12
LRRRLLLRLLRL
10
LLLLLRRRRR
9
LRLRLRLRL
```




```output1
3 5 5 
16 16 16 16 16 
0 
86 95 98 101 102 102 102 102 102 102 102 102 
29 38 45 52 57 62 65 68 69 70 
44 50 54 56 56 56 56 56 56
```



## Note

<p>In the first test case: </p><ul> <li> $k=1$: change the direction of $1$ person to make the line <span class="tex-font-style-tt">RLR</span>. The total value is $2+1+0=3$. </li><li> $k=2$: change the direction of $2$ people to make the line <span class="tex-font-style-tt">RLL</span>. The total value is $2+1+2=5$. </li><li> $k=3$: change the direction of $2$ people to make the line <span class="tex-font-style-tt">RLL</span>. The total value is $2+1+2=5$. Note that you have to change the direction of <span class="tex-font-style-bf">at most</span> $k$ people. </li></ul><p>In the second test case, it is optimal to only change the direction of the first person for all $k$ from $1$ to $5$ (that is, make the line <span class="tex-font-style-tt">RRRLL</span>).</p>
