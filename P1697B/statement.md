## Description

<div><p>The store sells $n$ items, the price of the $i$-th item is $p_i$. The store's management is going to hold a promotion: if a customer purchases at least $x$ items, $y$ cheapest of them are free.</p><p>The management has not yet decided on the exact values of $x$ and $y$. Therefore, they ask you to process $q$ queries: for the given values of $x$ and $y$, determine the maximum total value of items received for free, if a customer makes <span class="tex-font-style-bf">one purchase</span>.</p><p>Note that all queries are independent; they don't affect the store's stock.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;— the number of items in the store and the number of queries, respectively.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le 10^6$), where $p_i$&nbsp;— the price of the $i$-th item.</p><p>The following $q$ lines contain two integers $x_i$ and $y_i$ each ($1 \le y_i \le x_i \le n$)&nbsp;— the values of the parameters $x$ and $y$ in the $i$-th query.</p></div><div class="output-specification"><p>For each query, print a single integer&nbsp;— the maximum total value of items received for free <span class="tex-font-style-bf">for one purchase</span>.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;— the number of items in the store and the number of queries, respectively.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le 10^6$), where $p_i$&nbsp;— the price of the $i$-th item.</p><p>The following $q$ lines contain two integers $x_i$ and $y_i$ each ($1 \le y_i \le x_i \le n$)&nbsp;— the values of the parameters $x$ and $y$ in the $i$-th query.</p>

## Output

<p>For each query, print a single integer&nbsp;— the maximum total value of items received for free <span class="tex-font-style-bf">for one purchase</span>.</p>





```input1
5 3
5 3 1 5 2
3 2
1 1
5 3
```




```output1
8
5
6
```



## Note

<p>In the first query, a customer can buy three items worth $5, 3, 5$, the two cheapest of them are $3 + 5 = 8$.</p><p>In the second query, a customer can buy two items worth $5$ and $5$, the cheapest of them is $5$.</p><p>In the third query, a customer has to buy all the items to receive the three cheapest of them for free; their total price is $1 + 2 + 3 = 6$.</p>
