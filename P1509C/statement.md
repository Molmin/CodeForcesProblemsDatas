## Description

<div><p>The student council is preparing for the relay race at the sports festival.</p><p>The council consists of $n$ members. They will run one after the other in the race, the speed of member $i$ is $s_i$. The <span class="tex-font-style-it">discrepancy</span> $d_i$ of the $i$-th stage is the difference between the maximum and the minimum running speed among the first $i$ members who ran. Formally, if $a_i$ denotes the speed of the $i$-th member who participated in the race, then $d_i = \max(a_1, a_2, \dots, a_i) - \min(a_1, a_2, \dots, a_i)$.</p><p>You want to minimize the sum of the discrepancies $d_1 + d_2 + \dots + d_n$. To do this, you are allowed to change the order in which the members run. What is the minimum possible sum that can be achieved?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2000$) &nbsp;— the number of members of the student council.</p><p>The second line contains $n$ integers $s_1, s_2, \dots, s_n$ ($1 \le s_i \le 10^9$) &nbsp;– the running speeds of the members.</p></div><div class="output-specification"><p>Print a single integer &nbsp;— the minimum possible value of $d_1 + d_2 + \dots + d_n$ after choosing the order of the members.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2000$) &nbsp;— the number of members of the student council.</p><p>The second line contains $n$ integers $s_1, s_2, \dots, s_n$ ($1 \le s_i \le 10^9$) &nbsp;– the running speeds of the members.</p>

## Output

<p>Print a single integer &nbsp;— the minimum possible value of $d_1 + d_2 + \dots + d_n$ after choosing the order of the members.</p>





```input1
3
3 1 2
```




```input2
1
5
```




```input3
6
1 6 3 3 6 3
```




```input4
6
104 943872923 6589 889921234 1000000000 69
```




```output1
3
```




```output2
0
```




```output3
11
```




```output4
2833800505
```



## Note

<p>In the first test case, we may choose to make the third member run first, followed by the first member, and finally the second. Thus $a_1 = 2$, $a_2 = 3$, and $a_3 = 1$. We have:</p><ul> <li> $d_1 = \max(2) - \min(2) = 2 - 2 = 0$. </li><li> $d_2 = \max(2, 3) - \min(2, 3) = 3 - 2 = 1$. </li><li> $d_3 = \max(2, 3, 1) - \min(2, 3, 1) = 3 - 1 = 2$. </li></ul><p>The resulting sum is $d_1 + d_2 + d_3 = 0 + 1 + 2 = 3$. It can be shown that it is impossible to achieve a smaller value.</p><p>In the second test case, the only possible rearrangement gives $d_1 = 0$, so the minimum possible result is $0$.</p>
