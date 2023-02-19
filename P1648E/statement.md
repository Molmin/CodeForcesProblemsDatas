## Description

<div><p>Berland is a large country with developed airlines. In total, there are $n$ cities in the country that are historically served by the Berlaflot airline. The airline operates bi-directional flights between $m$ pairs of cities, $i$-th of them connects cities with numbers $a_i$ and $b_i$ and has a price $c_i$ for a flight in both directions.</p><p>It is known that Berlaflot flights can be used to get from any city to any other (possibly with transfers), and the cost of any route that consists of several consequent flights is equal to the cost of the most expensive of them. More formally, the cost of the route from a city $t_1$ to a city $t_k$ with $(k-2)$ transfers using cities $t_2,\ t_3,\ t_4,\ \ldots,\ t_{k - 1}$ is equal to the maximum cost of flights from $t_1$ to $t_2$, from $t_2$ to $t_3$, from $t_3$ to $t_4$ and so on until the flight from $t_{k - 1}$ to $t_k$. Of course, all these flights must be operated by Berlaflot.</p><p>A new airline, S8 Airlines, has recently started operating in Berland. This airline provides bi-directional flights between all pairs of cities that are not connected by Berlaflot direct flights. Thus, between each pair of cities there is a flight of either Berlaflot or S8 Airlines.</p><p>The cost of S8 Airlines flights is calculated as follows: for each pair of cities $x$ and $y$ that is connected by a S8 Airlines flight, the cost of this flight is equal to the minimum cost of the route between the cities $x$ and $y$ at Berlaflot according to the pricing described earlier.</p><p>It is known that with the help of S8 Airlines flights you can get from any city to any other with possible transfers, and, similarly to Berlaflot, the cost of a route between any two cities that consists of several S8 Airlines flights is equal to the cost of the most expensive flight.</p><p>Due to the increased competition with S8 Airlines, Berlaflot decided to introduce an air reform and change the costs of its flights. Namely, for the $i$-th of its flight between the cities $a_i$ and $b_i$, Berlaflot wants to make the cost of this flight equal to the minimum cost of the route between the cities $a_i$ and $b_i$ at S8 Airlines. Help Berlaflot managers calculate new flight costs.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains one integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the amount of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($4 \le n \le 200\,000$, $n - 1 \le m \le 200\,000$, $m \le \frac{(n - 1) (n - 2)}{2}$)&nbsp;— the amount of cities in Berland and the amount of Berlaflot flights.</p><p>The next $m$ lines contain the description of Berlaflot flights. The $i$-th line contains three integers $a_i$, $b_i$ and $c_i$ ($1 \le a_i, b_i \le n$, $1 \le c_i \le 10^9$)&nbsp;— the numbers of cities that are connected with $i$-th Berlaflot flight and the price of $i$-th Berlaflot flight.</p><p>It is guaranteed that no flight connects a city with itself, no two flights connect the same pair of cities. It is guaranteed that by using Berlaflot flights it is possible to get from any city to any other and by using S8 Airlines flights it is possible to get from any city to any other.</p><p>Let $N$ be the sum of $n$ over all test cases and $M$ be the sum of $m$ over all test cases. It is guaranteed that $N, M \le 200\,000$.</p></div><div class="output-specification"><p>For each test case you should print $m$ integers in a single line, $i$-th of them should be the price of $i$-th Berlaflot flight after the air reform.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains one integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the amount of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($4 \le n \le 200\,000$, $n - 1 \le m \le 200\,000$, $m \le \frac{(n - 1) (n - 2)}{2}$)&nbsp;— the amount of cities in Berland and the amount of Berlaflot flights.</p><p>The next $m$ lines contain the description of Berlaflot flights. The $i$-th line contains three integers $a_i$, $b_i$ and $c_i$ ($1 \le a_i, b_i \le n$, $1 \le c_i \le 10^9$)&nbsp;— the numbers of cities that are connected with $i$-th Berlaflot flight and the price of $i$-th Berlaflot flight.</p><p>It is guaranteed that no flight connects a city with itself, no two flights connect the same pair of cities. It is guaranteed that by using Berlaflot flights it is possible to get from any city to any other and by using S8 Airlines flights it is possible to get from any city to any other.</p><p>Let $N$ be the sum of $n$ over all test cases and $M$ be the sum of $m$ over all test cases. It is guaranteed that $N, M \le 200\,000$.</p>

## Output

<p>For each test case you should print $m$ integers in a single line, $i$-th of them should be the price of $i$-th Berlaflot flight after the air reform.</p>





```input1
3
4 3
1 2 1
2 3 2
4 3 3
5 5
1 2 1
1 3 1
2 4 1
4 5 2
5 1 3
6 6
1 2 3
2 3 1
3 6 5
3 4 2
4 5 4
2 4 2
```




```output1
3 3 3 
1 1 1 2 2 
4 4 5 3 4 4
```



## Note

<p>In the first test case S8 Airlines will provide flights between these pairs of cities: $(1, 3)$, $(1, 4)$ and $(2, 4)$.</p><p>The cost of a flight between cities $1$ and $3$ will be equal to $2$, since the minimum cost of the Berlaflot route is $2$&nbsp;— the route consists of a flight between cities $1$ and $2$ costing $1$ and a flight between cities $2$ and $3$ costing $2$, the maximum cost is $2$.</p><p>The cost of a flight between cities $1$ and $4$ will be $3$, since the minimum cost of the Berlaflot route is $3$&nbsp;— the route consists of a flight between cities $1$ and $2$ costing $1$, a flight between cities $2$ and $3$ costing $2$ and a flight between cities $3$ and $4$ costing $3$, the maximum cost is $3$.</p><p>The cost of a flight between cities $2$ and $4$ will be $3$, since the minimum cost of the Berlaflot route is $3$&nbsp;— the route consists of a flight between cities $2$ and $3$ costing $2$ and a flight between cities $3$ and $4$ costing $3$, the maximum cost is $3$.</p><p>After the air reform, the cost of the Berlaflot flight between cities $1$ and $2$ will be $3$, since the minimum cost of the S8 Airlines route between these cities is $3$&nbsp;— the route consists of a flight between cities $1$ and $4$ costing $3$ and a flight between cities $2$ and $4$ costing $3$, the maximum cost is $3$.</p><p>The cost of the Berlaflot flight between cities $2$ and $3$ will be $3$, since the minimum cost of the S8 Airlines route between these cities is $3$&nbsp;— the route consists of a flight between cities $2$ and $4$ costing $3$, a flight between cities $1$ and $4$ costing $3$ and a flight between $1$ and $3$ costing $2$, the maximum cost is $3$.</p><p>The cost of the Berlaflot flight between cities $3$ and $4$ will be $3$, since the minimum cost of the S8 Airlines route between these cities is $3$&nbsp;— the route consists of a flight between cities $1$ and $3$ costing $2$ and a flight between cities $1$ and $4$ costing $3$, the maximum cost is $3$. </p><p> In the second test case S8 Airlines will have the following flights: between cities $1$ and $4$ costing $1$, between cities $2$ and $3$ costing $1$, between cities $2$ and $5$ costing $2$, between cities $3$ and $4$ costing $1$ and between cities $3$ and $5$ costing $2$.</p>
