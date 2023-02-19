## Description

<div><p>You are given a permutation $p$ of length $n$ (a permutation of length $n$ is an array of length $n$ in which each integer from $1$ to $n$ occurs exactly once).</p><p>You can perform the following operation any number of times (possibly zero): </p><ol> <li> choose two different elements $x$ and $y$ and erase them from the permutation; </li><li> insert the minimum of $x$ and $y$ into the permutation in such a way that it becomes the first element; </li><li> insert the maximum of $x$ and $y$ into the permutation in such a way that it becomes the last element. </li></ol><p>For example, if $p = [1, 5, 4, 2, 3]$ and we want to apply the operation to the elements $3$ and $5$, then after the first step of the operation, the permutation becomes $p = [1, 4, 2]$; and after we insert the elements, it becomes $p = [3, 1, 4, 2, 5]$.</p><p>Your task is to calculate the minimum number of operations described above to sort the permutation $p$ in ascending order (i. e. transform $p$ so that $p_1 &lt; p_2 &lt; \dots &lt; p_n$).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of the test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of elements in the permutation.</p><p>The second line of the test case contains $n$ distinct integers from $1$ to $n$&nbsp;— the given permutation $p$.</p><p>The sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the minimum number of operations described above to sort the array $p$ in ascending order.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of the test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of elements in the permutation.</p><p>The second line of the test case contains $n$ distinct integers from $1$ to $n$&nbsp;— the given permutation $p$.</p><p>The sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the minimum number of operations described above to sort the array $p$ in ascending order.</p>





```input1|2,3,6,7
4
5
1 5 4 2 3
3
1 2 3
4
2 1 4 3
6
5 2 4 1 6 3
```




```output1
2
0
1
3
```



## Note

<p>In the first example, you can proceed as follows: </p><ol> <li> in the permutation $p = [1, 5, 4, 2, 3]$, let's choose the elements $4$ and $2$, then, after applying the operation, the permutation becomes $p = [2, 1, 5, 3, 4]$; </li><li> in the permutation $p = [2, 1, 5, 3, 4]$, let's choose the elements $1$ and $5$, then, after applying operation, the permutation becomes $p = [1, 2, 3, 4, 5]$. </li></ol>
