## Description

<div><p>Danny, the local Math Maniac, is fascinated by circles, Omkar's most recent creation. Help him solve this circle problem!</p><p>You are given $n$ nonnegative integers $a_1, a_2, \dots, a_n$ arranged in a circle, where $n$ must be odd (ie. $n-1$ is divisible by $2$). Formally, for all $i$ such that $2 \leq i \leq n$, the elements $a_{i - 1}$ and $a_i$ are considered to be adjacent, and $a_n$ and $a_1$ are also considered to be adjacent. In one operation, you pick a number on the circle, replace it with the sum of the two elements adjacent to it, and then delete the two adjacent elements from the circle. This is repeated until only one number remains in the circle, which we call the circular value.</p><p>Help Danny find the maximum possible circular value after some sequences of operations. </p></div><div class="input-specification"><p>The first line contains one odd integer $n$ ($1 \leq n &lt; 2 \cdot 10^5$, $n$ is odd) &nbsp;— the initial size of the circle.</p><p>The second line contains $n$ integers $a_{1},a_{2},\dots,a_{n}$ ($0 \leq a_{i} \leq 10^9$) &nbsp;— the initial numbers in the circle.</p></div><div class="output-specification"><p>Output the maximum possible circular value after applying some sequence of operations to the given circle.</p></div>

## Input

<p>The first line contains one odd integer $n$ ($1 \leq n &lt; 2 \cdot 10^5$, $n$ is odd) &nbsp;— the initial size of the circle.</p><p>The second line contains $n$ integers $a_{1},a_{2},\dots,a_{n}$ ($0 \leq a_{i} \leq 10^9$) &nbsp;— the initial numbers in the circle.</p>

## Output

<p>Output the maximum possible circular value after applying some sequence of operations to the given circle.</p>





```input1
3
7 10 2
```




```input2
1
4
```




```output1
17
```




```output2
4
```



## Note

<p>For the first test case, here's how a circular value of $17$ is obtained:</p><p>Pick the number at index $3$. The sum of adjacent elements equals $17$. Delete $7$ and $10$ from the circle and replace $2$ with $17$.</p><p>Note that the answer may not fit in a $32$-bit integer.</p>
