## Description

<div><p>You have a knapsack with the capacity of $W$. There are also $n$ items, the $i$-th one has weight $w_i$. </p><p>You want to put some of these items into the knapsack in such a way that their total weight $C$ is at least half of its size, but (obviously) does not exceed it. Formally, $C$ should satisfy: $\lceil \frac{W}{2}\rceil \le C \le W$. </p><p>Output the list of items you will put into the knapsack or determine that fulfilling the conditions is impossible. </p><p>If there are several possible lists of items satisfying the conditions, you can output any. Note that you <span class="tex-font-style-bf">don't</span> have to maximize the sum of weights of items in the knapsack.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains integers $n$ and $W$ ($1 \le n \le 200\,000$, $1\le W \le 10^{18}$). </p><p>The second line of each test case contains $n$ integers $w_1, w_2, \dots, w_n$ ($1 \le w_i \le 10^9$)&nbsp;— weights of the items.</p><p>The sum of $n$ over all test cases does not exceed $200\,000$.</p></div><div class="output-specification"><p>For each test case, if there is no solution, print a single integer $-1$. </p><p>If there exists a solution consisting of $m$ items, print $m$ in the first line of the output and $m$ integers $j_1$, $j_2$, ..., $j_m$ ($1 \le j_i \le n$, <span class="tex-font-style-bf">all $j_i$ are distinct</span>) in the second line of the output &nbsp;— indices of the items you would like to pack into the knapsack.</p><p>If there are several possible lists of items satisfying the conditions, you can output any. Note that you <span class="tex-font-style-bf">don't</span> have to maximize the sum of weights items in the knapsack.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains integers $n$ and $W$ ($1 \le n \le 200\,000$, $1\le W \le 10^{18}$). </p><p>The second line of each test case contains $n$ integers $w_1, w_2, \dots, w_n$ ($1 \le w_i \le 10^9$)&nbsp;— weights of the items.</p><p>The sum of $n$ over all test cases does not exceed $200\,000$.</p>

## Output

<p>For each test case, if there is no solution, print a single integer $-1$. </p><p>If there exists a solution consisting of $m$ items, print $m$ in the first line of the output and $m$ integers $j_1$, $j_2$, ..., $j_m$ ($1 \le j_i \le n$, <span class="tex-font-style-bf">all $j_i$ are distinct</span>) in the second line of the output &nbsp;— indices of the items you would like to pack into the knapsack.</p><p>If there are several possible lists of items satisfying the conditions, you can output any. Note that you <span class="tex-font-style-bf">don't</span> have to maximize the sum of weights items in the knapsack.</p>





```input1
3
1 3
3
6 2
19 8 19 69 9 4
7 12
1 1 1 17 1 1 1
```




```output1
1
1
-1
6
1 2 3 5 6 7
```



## Note

<p>In the first test case, you can take the item of weight $3$ and fill the knapsack just right.</p><p>In the second test case, all the items are larger than the knapsack's capacity. Therefore, the answer is $-1$.</p><p>In the third test case, you fill the knapsack exactly in half.</p>
