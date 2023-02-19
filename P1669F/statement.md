## Description

<div><p>There are $n$ candies put from left to right on a table. The candies are numbered from left to right. The $i$-th candy has weight $w_i$. Alice and Bob eat candies. </p><p>Alice can eat any number of candies from the left (she can't skip candies, she eats them in a row). </p><p>Bob can eat any number of candies from the right (he can't skip candies, he eats them in a row). </p><p>Of course, if Alice ate a candy, Bob can't eat it (and vice versa).</p><p>They want to be fair. Their goal is to eat the same total weight of candies. What is the most number of candies they can eat in total?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the number of candies on the table.</p><p>The second line of each test case contains $n$ integers $w_1, w_2, \dots, w_n$ ($1 \leq w_i \leq 10^4$)&nbsp;— the weights of candies from left to right.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the maximum number of candies Alice and Bob can eat in total while satisfying the condition.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the number of candies on the table.</p><p>The second line of each test case contains $n$ integers $w_1, w_2, \dots, w_n$ ($1 \leq w_i \leq 10^4$)&nbsp;— the weights of candies from left to right.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the maximum number of candies Alice and Bob can eat in total while satisfying the condition.</p>





```input1
4
3
10 20 10
6
2 1 4 2 4 1
5
1 2 4 8 16
9
7 3 20 5 15 1 11 8 10
```




```output1
2
6
0
7
```



## Note

<p>For the first test case, Alice will eat one candy from the left and Bob will eat one candy from the right. There is no better way for them to eat the same total amount of weight. The answer is $2$ because they eat two candies in total.</p><p>For the second test case, Alice will eat the first three candies from the left (with total weight $7$) and Bob will eat the first three candies from the right (with total weight $7$). They cannot eat more candies since all the candies have been eaten, so the answer is $6$ (because they eat six candies in total).</p><p>For the third test case, there is no way Alice and Bob will eat the same non-zero weight so the answer is $0$.</p><p>For the fourth test case, Alice will eat candies with weights $[7, 3, 20]$ and Bob will eat candies with weights $[10, 8, 11, 1]$, they each eat $30$ weight. There is no better partition so the answer is $7$.</p>
