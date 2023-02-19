## Description

<div><p>Chef Monocarp has just put $n$ dishes into an oven. He knows that the $i$-th dish has its optimal cooking time equal to $t_i$ minutes.</p><p>At any <span class="tex-font-style-bf">positive integer</span> minute $T$ Monocarp can put <span class="tex-font-style-bf">no more than one</span> dish out of the oven. If the $i$-th dish is put out at some minute $T$, then its unpleasant value is $|T - t_i|$&nbsp;— the absolute difference between $T$ and $t_i$. Once the dish is out of the oven, it can't go back in.</p><p>Monocarp should put all the dishes out of the oven. What is the minimum total unpleasant value Monocarp can obtain?</p></div><div class="input-specification"><p>The first line contains a single integer $q$ ($1 \le q \le 200$)&nbsp;— the number of testcases.</p><p>Then $q$ testcases follow.</p><p>The first line of the testcase contains a single integer $n$ ($1 \le n \le 200$)&nbsp;— the number of dishes in the oven.</p><p>The second line of the testcase contains $n$ integers $t_1, t_2, \dots, t_n$ ($1 \le t_i \le n$)&nbsp;— the optimal cooking time for each dish.</p><p>The sum of $n$ over all $q$ testcases doesn't exceed $200$.</p></div><div class="output-specification"><p>Print a single integer for each testcase&nbsp;— the minimum total unpleasant value Monocarp can obtain when he puts out all the dishes out of the oven. Remember that Monocarp can only put the dishes out at positive integer minutes and no more than one dish at any minute.</p></div>

## Input

<p>The first line contains a single integer $q$ ($1 \le q \le 200$)&nbsp;— the number of testcases.</p><p>Then $q$ testcases follow.</p><p>The first line of the testcase contains a single integer $n$ ($1 \le n \le 200$)&nbsp;— the number of dishes in the oven.</p><p>The second line of the testcase contains $n$ integers $t_1, t_2, \dots, t_n$ ($1 \le t_i \le n$)&nbsp;— the optimal cooking time for each dish.</p><p>The sum of $n$ over all $q$ testcases doesn't exceed $200$.</p>

## Output

<p>Print a single integer for each testcase&nbsp;— the minimum total unpleasant value Monocarp can obtain when he puts out all the dishes out of the oven. Remember that Monocarp can only put the dishes out at positive integer minutes and no more than one dish at any minute.</p>





```input1
6
6
4 2 4 4 5 2
7
7 7 7 7 7 7 7
1
1
5
5 1 2 4 3
4
1 4 4 4
21
21 8 1 4 1 5 21 1 8 21 11 21 11 3 12 8 19 15 9 11 13
```




```output1
4
12
0
0
2
21
```



## Note

<p>In the first example Monocarp can put out the dishes at minutes $3, 1, 5, 4, 6, 2$. That way the total unpleasant value will be $|4 - 3| + |2 - 1| + |4 - 5| + |4 - 4| + |6 - 5| + |2 - 2| = 4$.</p><p>In the second example Monocarp can put out the dishes at minutes $4, 5, 6, 7, 8, 9, 10$.</p><p>In the third example Monocarp can put out the dish at minute $1$.</p><p>In the fourth example Monocarp can put out the dishes at minutes $5, 1, 2, 4, 3$.</p><p>In the fifth example Monocarp can put out the dishes at minutes $1, 3, 4, 5$.</p>
