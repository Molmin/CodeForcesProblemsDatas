## Description

<div><p>You are given an array of $n$ integers $a_1, a_2, \ldots, a_n$. The integers are either $1$ or $-1$. You have to perform the following operation <span class="tex-font-style-bf">exactly once</span> on the array $a$:</p><ul> <li> Choose an index $i$ ($1 \leq i &lt; n$) and flip the signs of $a_i$ and $a_{i+1}$. Here, flipping the sign means $-1$ will be $1$ and $1$ will be $-1$. </li></ul><p>What is the maximum possible value of $a_1 + a_2 + \ldots + a_n$ after applying the above operation?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$), the length of the array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($a_i = 1$ or $a_i = -1$).</p><p>The sum of $n$ over all cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the maximum possible sum of the array $a$ you can get in a separate line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$), the length of the array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($a_i = 1$ or $a_i = -1$).</p><p>The sum of $n$ over all cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print the maximum possible sum of the array $a$ you can get in a separate line.</p>





```input1|2,3,6,7
4
5
-1 1 1 -1 -1
5
1 1 -1 -1 -1
2
1 1
4
1 -1 -1 1
```




```output1
3
3
-2
4
```



## Note

<p>In the first case, we can choose index $4$ and flip the signs of $a_4$ and $a_5$. After this operation, the sum will be $-1+1+1+1+1 = 3$. We can't make the sum larger than this.</p><p>In the third case, the only option is to choose the index $1$.</p>
