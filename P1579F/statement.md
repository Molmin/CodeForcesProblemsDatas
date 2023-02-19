## Description

<div><p>You are given an array $a[0 \ldots n - 1] = [a_0, a_1, \ldots, a_{n - 1}]$ of zeroes and ones only. Note that in this problem, unlike the others, the array indexes are numbered from zero, not from one.</p><p>In one step, the array $a$ is replaced by another array of length $n$ according to the following rules: </p><ol> <li> First, a new array $a^{\rightarrow d}$ is defined as a cyclic shift of the array $a$ to the right by $d$ cells. The elements of this array can be defined as $a^{\rightarrow d}_i = a_{(i + n - d) \bmod n}$, where $(i + n - d) \bmod n$ is the remainder of integer division of $i + n - d$ by $n$. <p> It means that the whole array $a^{\rightarrow d}$ can be represented as a sequence $$a^{\rightarrow d} = [a_{n - d}, a_{n - d + 1}, \ldots, a_{n - 1}, a_0, a_1, \ldots, a_{n - d - 1}]$$</p><p> </p></li><li> Then each element of the array $a_i$ is replaced by $a_i \,\&amp;\, a^{\rightarrow d}_i$, where $\&amp;$ is a logical "AND" operator. </li></ol><p>For example, if $a = [0, 0, 1, 1]$ and $d = 1$, then $a^{\rightarrow d} = [1, 0, 0, 1]$ and the value of $a$ after the first step will be $[0 \,\&amp;\, 1, 0 \,\&amp;\, 0, 1 \,\&amp;\, 0, 1 \,\&amp;\, 1]$, that is $[0, 0, 0, 1]$.</p><p>The process ends when the array stops changing. For a given array $a$, determine whether it will consist of only zeros at the end of the process. If yes, also find the number of steps the process will take before it finishes.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases. </p><p>The first line of each test case description contains two integers: $n$ ($1 \le n \le 10^6$)&nbsp;— array size and $d$ ($1 \le d \le n$)&nbsp;— cyclic shift offset. The second line of the description contains $n$ space-separated integers $a_i$ ($0 \le a_i \le 1$)&nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should be a single integer&nbsp;— the number of steps after which the array will contain only zeros for the first time. If there are still elements equal to $1$ in the array after the end of the process, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases. </p><p>The first line of each test case description contains two integers: $n$ ($1 \le n \le 10^6$)&nbsp;— array size and $d$ ($1 \le d \le n$)&nbsp;— cyclic shift offset. The second line of the description contains $n$ space-separated integers $a_i$ ($0 \le a_i \le 1$)&nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should be a single integer&nbsp;— the number of steps after which the array will contain only zeros for the first time. If there are still elements equal to $1$ in the array after the end of the process, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5
2 1
0 1
3 2
0 1 0
5 2
1 1 0 1 0
4 2
0 1 0 1
1 1
0
```




```output1
1
1
3
-1
0
```



## Note

<p>In the third sample test case the array will change as follows: </p><ol> <li> At the beginning $a = [1, 1, 0, 1, 0]$, and $a^{\rightarrow 2} = [1, 0, 1, 1, 0]$. Their element-by-element "AND" is equal to $$[1 \,\&amp;\, 1, 1 \,\&amp;\, 0, 0 \,\&amp;\, 1, 1 \,\&amp;\, 1, 0 \,\&amp;\, 0] = [1, 0, 0, 1, 0]$$ </li><li> Now $a = [1, 0, 0, 1, 0]$, then $a^{\rightarrow 2} = [1, 0, 1, 0, 0]$. Their element-by-element "AND" equals to $$[1 \,\&amp;\, 1, 0 \,\&amp;\, 0, 0 \,\&amp;\, 1, 1 \,\&amp;\, 0, 0 \,\&amp;\, 0] = [1, 0, 0, 0, 0]$$ </li><li> And finally, when $a = [1, 0, 0, 0, 0]$ we get $a^{\rightarrow 2} = [0, 0, 1, 0, 0]$. Their element-by-element "AND" equals to $$[1 \,\&amp;\, 0, 0 \,\&amp;\, 0, 0 \,\&amp;\, 1, 0 \,\&amp;\, 0, 0 \,\&amp;\, 0] = [0, 0, 0, 0, 0]$$ </li></ol> Thus, the answer is $3$ steps.<p>In the fourth sample test case, the array will not change as it shifts by $2$ to the right, so each element will be calculated as $0 \,\&amp;\, 0$ or $1 \,\&amp;\, 1$ thus not changing its value. So the answer is <span class="tex-font-style-tt">-1</span>, the array will never contain only zeros.</p>
