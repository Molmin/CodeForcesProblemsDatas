## Description

<div><p>You are given an array of $n$ integers $a_1, a_2, \dots, a_n$</p><p>You can apply the following operation an arbitrary number of times: </p><ul> <li> select an index $i$ ($1 \le i \le n$) and replace the value of the element $a_i$ with the value $a_i + (a_i \bmod 10)$, where $a_i \bmod 10$ is the remainder of the integer dividing $a_i$ by $10$. </li></ul><p>For a single index (value $i$), this operation can be applied multiple times. If the operation is applied repeatedly to the same index, then the current value of $a_i$ is taken into account each time. For example, if $a_i=47$ then after the first operation we get $a_i=47+7=54$, and after the second operation we get $a_i=54+4=58$.</p><p>Check if it is possible to make <span class="tex-font-style-bf">all</span> array elements equal by applying multiple (possibly zero) operations.</p><p>For example, you have an array $[6, 11]$. </p><ul> <li> Let's apply this operation to the first element of the array. Let's replace $a_1 = 6$ with $a_1 + (a_1 \bmod 10) = 6 + (6 \bmod 10) = 6 + 6 = 12$. We get the array $[12, 11]$. </li><li> Then apply this operation to the second element of the array. Let's replace $a_2 = 11$ with $a_2 + (a_2 \bmod 10) = 11 + (11 \bmod 10) = 11 + 1 = 12$. We get the array $[12, 12]$. </li></ul><p>Thus, by applying $2$ operations, you can make all elements of an array equal.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. What follows is a description of each test case.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \le a_i \le 10^9$)&nbsp;— array elements.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if it is possible to make all array elements equal; </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can print <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer) .</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. What follows is a description of each test case.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \le a_i \le 10^9$)&nbsp;— array elements.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if it is possible to make all array elements equal; </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can print <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive answer) .</p>





```input1|2,3,6,7,10,11,14,15,18,19
10
2
6 11
3
2 18 22
5
5 10 5 10 5
4
1 2 4 8
2
4 5
3
93 96 102
2
40 6
2
50 30
2
22 44
2
1 5
```




```output1
Yes
No
Yes
Yes
No
Yes
No
No
Yes
No
```



## Note

<p>The first test case is clarified above.</p><p>In the second test case, it is impossible to make all array elements equal.</p><p>In the third test case, you need to apply this operation once to all elements equal to $5$.</p><p>In the fourth test case, you need to apply this operation to all elements until they become equal to $8$.</p><p>In the fifth test case, it is impossible to make all array elements equal.</p><p>In the sixth test case, you need to apply this operation to all elements until they become equal to $102$.</p>
