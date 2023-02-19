## Description

<div><p>Monocarp and Polycarp are working as waiters in Berpizza, a pizzeria located near the center of Bertown. Since they are waiters, their job is to serve the customers, but they choose whom they serve first differently.</p><p>At the start of the working day, there are no customers at the Berpizza. They come there one by one. When a customer comes into the pizzeria, she sits and waits for Monocarp or Polycarp to serve her. Monocarp has been working in Berpizza for just two weeks, so whenever he serves a customer, he simply chooses the one who came to Berpizza first, and serves that customer. </p><p>On the other hand, Polycarp is an experienced waiter at Berpizza, and he knows which customers are going to spend a lot of money at the pizzeria (and which aren't) as soon as he sees them. For each customer, Polycarp estimates the amount of money this customer can spend, and when he serves a customer, he chooses the one that is expected to leave the most money at Berpizza (in case there are several such customers, he chooses the one who came first among them). </p><p>Obviously, no customer can be served twice, so Monocarp and Polycarp choose which customer to serve only among those who haven't been served yet.</p><p>When the number of customers gets really high, it becomes difficult for both Monocarp and Polycarp to choose the customer they are going to serve. Your task is to write a program that makes these choices for them. Formally, your program should be able to process three types of queries:</p><ul> <li> $1$ $m$ — a customer comes to Berpizza, and Polycarp estimates the amount of money that they will spend as $m$; </li><li> $2$ — Monocarp serves a customer which came to the pizzeria first; </li><li> $3$ — Polycarp serves a customer which is expected to spend the largest amount of money at the pizzeria (if there are several such customers, the one that came to the pizzeria first is chosen). </li></ul><p>For each query of types $2$ and $3$, report the number of the customer who was served (the customers are numbered in the order they come to the pizzeria, starting from $1$).</p></div><div class="input-specification"><p>The first line contains one integer $q$ ($2 \le q \le 5 \cdot 10^5$) — the number of queries.</p><p>Then $q$ lines follow, each describing a query in one of the following formats:</p><ul> <li> $1$ $m$ ($1 \le m \le 5 \cdot 10^5$) — a customer comes to Berpizza, and Polycarp estimates the amount of money that they will spend as $m$; </li><li> $2$ — Monocarp serves a customer which came to the pizzeria first; </li><li> $3$ — Polycarp serves a customer which is expected to spend the largest amount of money at the pizzeria (if there are multiple such customers, the one that came to the pizzeria first is chosen). </li></ul><p>Queries of type $2$ and $3$ are asked only when there exists at least one customer that hasn't been served yet. There is at least one query of type $2$ or $3$ in the input.</p></div><div class="output-specification"><p>For each query of type $2$ or $3$, print one integer — the number of the customer that has been served in that event. The customers are numbered in the order in which they come to the pizzeria, starting from $1$.</p></div>

## Input

<p>The first line contains one integer $q$ ($2 \le q \le 5 \cdot 10^5$) — the number of queries.</p><p>Then $q$ lines follow, each describing a query in one of the following formats:</p><ul> <li> $1$ $m$ ($1 \le m \le 5 \cdot 10^5$) — a customer comes to Berpizza, and Polycarp estimates the amount of money that they will spend as $m$; </li><li> $2$ — Monocarp serves a customer which came to the pizzeria first; </li><li> $3$ — Polycarp serves a customer which is expected to spend the largest amount of money at the pizzeria (if there are multiple such customers, the one that came to the pizzeria first is chosen). </li></ul><p>Queries of type $2$ and $3$ are asked only when there exists at least one customer that hasn't been served yet. There is at least one query of type $2$ or $3$ in the input.</p>

## Output

<p>For each query of type $2$ or $3$, print one integer — the number of the customer that has been served in that event. The customers are numbered in the order in which they come to the pizzeria, starting from $1$.</p>





```input1
8
1 8
1 10
1 6
3
2
1 9
2
3
```




```input2
6
1 8
1 10
1 8
3
3
3
```




```input3
8
1 103913
3
1 103913
1 103913
3
1 103913
1 103913
2
```




```output1
2 1 3 4
```




```output2
2 1 3
```




```output3
1 2 3
```


