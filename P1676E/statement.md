## Description

<div><p>Timur has $n$ candies. The $i$-th candy has a quantity of sugar equal to $a_i$. So, by eating the $i$-th candy, Timur consumes a quantity of sugar equal to $a_i$.</p><p>Timur will ask you $q$ queries regarding his candies. For the $j$-th query you have to answer what is the <span class="tex-font-style-bf">minimum</span> number of candies he needs to eat in order to reach a quantity of sugar <span class="tex-font-style-bf">greater than or equal to</span> $x_j$ or print <span class="tex-font-style-tt">-1</span> if it's not possible to obtain such a quantity. In other words, you should print the minimum possible $k$ such that after eating $k$ candies, Timur consumes a quantity of sugar of at least $x_j$ or say that no possible $k$ exists.</p><p>Note that he can't eat the same candy twice and queries are independent of each other (Timur can use the same candy in different queries).</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \leq t \leq 1000$) &nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line contains $2$ integers $n$ and $q$ ($1 \leq n, q \leq 1.5\cdot10^5$)&nbsp;— the number of candies Timur has and the number of queries you have to print an answer for respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^4$)&nbsp;— the quantity of sugar in each of the candies respectively.</p><p>Then $q$ lines follow. </p><p>Each of the next $q$ lines contains a single integer $x_j$ ($1 \leq x_j \leq 2 \cdot 10^9$)&nbsp;– the quantity Timur wants to reach for the given query.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ over all test cases do not exceed $1.5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output $q$ lines. For the $j$-th line output the number of candies Timur needs to eat in order to reach a quantity of sugar greater than or equal to $x_j$ or print <span class="tex-font-style-tt">-1</span> if it's not possible to obtain such a quantity.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \leq t \leq 1000$) &nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line contains $2$ integers $n$ and $q$ ($1 \leq n, q \leq 1.5\cdot10^5$)&nbsp;— the number of candies Timur has and the number of queries you have to print an answer for respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^4$)&nbsp;— the quantity of sugar in each of the candies respectively.</p><p>Then $q$ lines follow. </p><p>Each of the next $q$ lines contains a single integer $x_j$ ($1 \leq x_j \leq 2 \cdot 10^9$)&nbsp;– the quantity Timur wants to reach for the given query.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ over all test cases do not exceed $1.5 \cdot 10^5$.</p>

## Output

<p>For each test case output $q$ lines. For the $j$-th line output the number of candies Timur needs to eat in order to reach a quantity of sugar greater than or equal to $x_j$ or print <span class="tex-font-style-tt">-1</span> if it's not possible to obtain such a quantity.</p>





```input1
3
8 7
4 3 3 1 1 4 5 9
1
10
50
14
15
22
30
4 1
1 2 3 4
3
1 2
5
4
6
```




```output1
1
2
-1
2
3
4
8
1
1
-1
```



## Note

<p>For the first test case:</p><p>For the first query, Timur can eat any candy, and he will reach the desired quantity.</p><p>For the second query, Timur can reach a quantity of at least $10$ by eating the $7$-th and the $8$-th candies, thus consuming a quantity of sugar equal to $14$.</p><p>For the third query, there is no possible answer.</p><p>For the fourth query, Timur can reach a quantity of at least $14$ by eating the $7$-th and the $8$-th candies, thus consuming a quantity of sugar equal to $14$.</p><p>For the second test case:</p><p>For the only query of the second test case, we can choose the third candy from which Timur receives exactly $3$ sugar. It's also possible to obtain the same answer by choosing the fourth candy.</p>
