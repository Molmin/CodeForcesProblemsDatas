## Description

<div><p>Vlad has $n$ friends, for each of whom he wants to buy <span class="tex-font-style-it">one</span> gift for the New Year.</p><p>There are $m$ shops in the city, in each of which he can buy a gift for any of his friends. If the $j$-th friend ($1 \le j \le n$) receives a gift bought in the shop with the number $i$ ($1 \le i \le m$), then the friend receives $p_{ij}$ units of joy. The rectangular table $p_{ij}$ is given in the input.</p><p>Vlad has time to visit at most $n-1$ shops (where $n$ is the number of <span class="tex-font-style-bf">friends</span>). He chooses which shops he will visit and for which friends he will buy gifts in each of them.</p><p>Let the $j$-th friend receive $a_j$ units of joy from Vlad's gift. Let's find the value $\alpha=\min\{a_1, a_2, \dots, a_n\}$. Vlad's goal is to buy gifts so that the value of $\alpha$ is as large as possible. In other words, Vlad wants to maximize the minimum of the joys of his friends.</p><p>For example, let $m = 2$, $n = 2$. Let the joy from the gifts that we can buy in the first shop: $p_{11} = 1$, $p_{12}=2$, in the second shop: $p_{21} = 3$, $p_{22}=4$.</p><p>Then it is enough for Vlad to go only to the second shop and buy a gift for the first friend, bringing joy $3$, and for the second&nbsp;— bringing joy $4$. In this case, the value $\alpha$ will be equal to $\min\{3, 4\} = 3$</p><p>Help Vlad choose gifts for his friends so that the value of $\alpha$ is as high as possible. Please note that each friend must receive one gift. Vlad can visit at most $n-1$ shops (where $n$ is the number of <span class="tex-font-style-bf">friends</span>). In the shop, he can buy any number of gifts.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input.</p><p>An empty line is written before each test case. Then there is a line containing integers $m$ and $n$ ($2 \le n$, $2 \le n \cdot m \le 10^5$) separated by a space&nbsp;— the number of shops and the number of friends, where $n \cdot m$ is the product of $n$ and $m$.</p><p>Then $m$ lines follow, each containing $n$ numbers. The number in the $i$-th row of the $j$-th column $p_{ij}$ ($1 \le p_{ij} \le 10^9$) is the joy of the product intended for friend number $j$ in shop number $i$.</p><p>It is guaranteed that the sum of the values $n \cdot m$ over all test cases in the test does not exceed $10^5$.</p></div><div class="output-specification"><p>Print $t$ lines, each line must contain the answer to the corresponding test case&nbsp;— the maximum possible value of $\alpha$, where $\alpha$ is the minimum of the joys from a gift for all of Vlad's friends.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input.</p><p>An empty line is written before each test case. Then there is a line containing integers $m$ and $n$ ($2 \le n$, $2 \le n \cdot m \le 10^5$) separated by a space&nbsp;— the number of shops and the number of friends, where $n \cdot m$ is the product of $n$ and $m$.</p><p>Then $m$ lines follow, each containing $n$ numbers. The number in the $i$-th row of the $j$-th column $p_{ij}$ ($1 \le p_{ij} \le 10^9$) is the joy of the product intended for friend number $j$ in shop number $i$.</p><p>It is guaranteed that the sum of the values $n \cdot m$ over all test cases in the test does not exceed $10^5$.</p>

## Output

<p>Print $t$ lines, each line must contain the answer to the corresponding test case&nbsp;— the maximum possible value of $\alpha$, where $\alpha$ is the minimum of the joys from a gift for all of Vlad's friends.</p>





```input1
5

2 2
1 2
3 4

4 3
1 3 1
3 1 1
1 2 2
1 1 3

2 3
5 3 4
2 5 1

4 2
7 9
8 1
9 6
10 8

2 4
6 5 2 1
7 9 7 2
```




```output1
3
2
4
8
2
```


