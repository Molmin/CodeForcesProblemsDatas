## Description

<div><p>A group of $n$ friends decide to go to a restaurant. Each of the friends plans to order meals for $x_i$ burles and has a total of $y_i$ burles ($1 \le i \le n$). </p><p>The friends decide to split their visit to the restaurant into several days. Each day, some group of <span class="tex-font-style-bf">at least two</span> friends goes to the restaurant. Each of the friends visits the restaurant no more than once (that is, these groups do not intersect). These groups must satisfy the condition that the total budget of each group must be <span class="tex-font-style-bf">not less</span> than the amount of burles that the friends in the group are going to spend at the restaurant. In other words, the sum of all $x_i$ values in the group must not exceed the sum of $y_i$ values in the group.</p><p>What is the maximum number of days friends can visit the restaurant?</p><p>For example, let there be $n = 6$ friends for whom $x$ = [$8, 3, 9, 2, 4, 5$] and $y$ = [$5, 3, 1, 4, 5, 10$]. Then: </p><ul> <li> first and sixth friends can go to the restaurant on the first day. They will spend $8+5=13$ burles at the restaurant, and their total budget is $5+10=15$ burles. Since $15 \ge 13$, they can actually form a group. </li><li> friends with indices $2, 4, 5$ can form a second group. They will spend $3+2+4=9$ burles at the restaurant, and their total budget will be $3+4+5=12$ burles ($12 \ge 9$). </li></ul><p>It can be shown that they will not be able to form more groups so that each group has at least two friends and each group can pay the bill.</p><p>So, the maximum number of groups the friends can split into is $2$. Friends will visit the restaurant for a maximum of two days. Note that the $3$-rd friend will not visit the restaurant at all.</p><p>Output the maximum number of days the friends can visit the restaurant for given $n$, $x$ and $y$.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$) — the number of friends.</p><p>The second line of each test case contains exactly $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_i \le 10^9$). The value of $x_i$ corresponds to the number of burles that the friend numbered $i$ plans to spend at the restaurant.</p><p>The third line of each test case contains exactly $n$ integers $y_1, y_2, \dots, y_n$ ($1 \le y_i \le 10^9$). The value $y_i$ corresponds to the number of burles that the friend numbered $i$ has.</p><p>It is guaranteed that the sum of $n$ values over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the maximum number of days to visit the restaurant. If friends cannot form even one group to visit the restaurant, print <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$) — the number of friends.</p><p>The second line of each test case contains exactly $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_i \le 10^9$). The value of $x_i$ corresponds to the number of burles that the friend numbered $i$ plans to spend at the restaurant.</p><p>The third line of each test case contains exactly $n$ integers $y_1, y_2, \dots, y_n$ ($1 \le y_i \le 10^9$). The value $y_i$ corresponds to the number of burles that the friend numbered $i$ has.</p><p>It is guaranteed that the sum of $n$ values over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print the maximum number of days to visit the restaurant. If friends cannot form even one group to visit the restaurant, print <span class="tex-font-style-tt">0</span>.</p>





```input1|2,3,4,8,9,10,14,15,16
6
6
8 3 9 2 4 5
5 3 1 4 5 10
4
1 2 3 4
1 1 2 2
3
2 3 7
1 3 10
6
2 3 6 9 5 7
3 2 7 10 6 10
6
5 4 2 1 8 100
1 1 1 1 1 200
6
1 4 1 2 4 2
1 3 3 2 3 4
```




```output1
2
0
1
3
1
3
```



## Note

<p>The first test case in explained in the problem statement.</p><p>In the second test case, friends cannot form at least one group of two or more people.</p><p>In the third test case, one way to visit the restaurant in one day is to go in a group of all three friends ($1+3+10 \ge 2+3+7$). Note that they do not have the option of splitting into two groups.</p>
