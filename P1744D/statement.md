## Description

<div><p>You are given an array of positive integers $a_1, a_2, \ldots, a_n$.</p><p>Make the product of all the numbers in the array (that is, $a_1 \cdot a_2 \cdot \ldots \cdot a_n$) divisible by $2^n$.</p><p>You can perform the following operation as many times as you like:</p><ul> <li> select an arbitrary index $i$ ($1 \leq i \leq n$) and replace the value $a_i$ with $a_i=a_i \cdot i$. </li></ul><p>You cannot apply the operation repeatedly to a single index. In other words, all selected values of $i$ must be different.</p><p>Find the smallest number of operations you need to perform to make the product of all the elements in the array divisible by $2^n$. Note that such a set of operations does not always exist.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ $(1 \leq t \leq 10^4$) — the number test cases.</p><p>Then the descriptions of the input data sets follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) — the length of array $a$.</p><p>The second line of each test case contains exactly $n$ integers: $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ values over all test cases in a test does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the least number of operations to make the product of all numbers in the array divisible by $2^n$. If the answer does not exist, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ $(1 \leq t \leq 10^4$) — the number test cases.</p><p>Then the descriptions of the input data sets follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) — the length of array $a$.</p><p>The second line of each test case contains exactly $n$ integers: $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ values over all test cases in a test does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the least number of operations to make the product of all numbers in the array divisible by $2^n$. If the answer does not exist, print <span class="tex-font-style-tt">-1</span>.</p>





```input1|2,3,6,7,10,11
6
1
2
2
3 2
3
10 6 11
4
13 17 1 1
5
1 1 12 1 1
6
20 7 14 18 3 5
```




```output1
0
1
1
-1
2
1
```



## Note

<p>In the first test case, the product of all elements is initially $2$, so no operations needed.</p><p>In the second test case, the product of elements initially equals $6$. We can apply the operation for $i = 2$, and then $a_2$ becomes $2\cdot2=4$, and the product of numbers becomes $3\cdot4=12$, and this product of numbers is divided by $2^n=2^2=4$. </p><p>In the fourth test case, even if we apply all possible operations, we still cannot make the product of numbers divisible by $2^n$ &nbsp;— it will be $(13\cdot1)\cdot(17\cdot2)\cdot(1\cdot3)\cdot(1\cdot4)=5304$, which does not divide by $2^n=2^4=16$.</p><p>In the fifth test case, we can apply operations for $i = 2$ and $i = 4$. </p>
