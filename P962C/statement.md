## Description

<div><p>You are given a positive integer $n$, written without leading zeroes (for example, the number <span class="tex-font-style-tt">04</span> is incorrect). </p><p>In one operation you can delete any digit of the given integer so that the result remains a positive integer without leading zeros.</p><p>Determine the minimum number of operations that you need to consistently apply to the given integer $n$ to make from it the square of some positive integer or report that it is impossible.</p><p>An integer $x$ is the square of some positive integer if and only if $x=y^2$ for some positive integer $y$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^{9}$). The number is given without leading zeroes.</p></div><div class="output-specification"><p>If it is impossible to make the square of some positive integer from $n$, print <span class="tex-font-style-tt">-1</span>. In the other case, print the minimal number of operations required to do it.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^{9}$). The number is given without leading zeroes.</p>

## Output

<p>If it is impossible to make the square of some positive integer from $n$, print <span class="tex-font-style-tt">-1</span>. In the other case, print the minimal number of operations required to do it.</p>





```input1
8314

```




```input2
625

```




```input3
333

```




```output1
2

```




```output2
0

```




```output3
-1

```



## Note

<p>In the first example we should delete from $8314$ the digits $3$ and $4$. After that $8314$ become equals to $81$, which is the square of the integer $9$.</p><p>In the second example the given $625$ is the square of the integer $25$, so you should not delete anything. </p><p>In the third example it is impossible to make the square from $333$, so the answer is <span class="tex-font-style-tt">-1</span>.</p>
