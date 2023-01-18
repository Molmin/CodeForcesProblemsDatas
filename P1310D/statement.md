## Description

<div><p>Masha lives in a country with $n$ cities numbered from $1$ to $n$. She lives in the city number $1$. </p><p>There is a direct train <span class="tex-font-style-it">route</span> between each pair of distinct cities $i$ and $j$, where $i \neq j$. In total there are $n(n-1)$ distinct routes. Every route has a cost, cost for route from $i$ to $j$ may be different from the cost of route from $j$ to $i$.</p><p>Masha wants to start her journey in city $1$, take <span class="tex-font-style-bf">exactly</span> $k$ routes from one city to another and as a result return to the city $1$. Masha is really careful with money, so she wants the journey to be as cheap as possible. To do so Masha doesn't mind visiting a city multiple times or even taking the same route multiple times.</p><p>Masha doesn't want her journey to have odd cycles. Formally, if you can select visited by Masha city $v$, take <span class="tex-font-style-bf">odd</span> number of routes used by Masha in her journey and return to the city $v$, such journey is considered unsuccessful.</p><p>Help Masha to find the cheapest (with minimal total cost of all taken routes) successful journey.</p></div><div class="input-specification"><p>First line of input had two integer numbers $n,k$ ($2 \leq n \leq 80; 2 \leq k \leq 10$): number of cities in the country and number of routes in Masha's journey. It is guaranteed that $k$ is even.</p><p>Next $n$ lines hold route descriptions: $j$-th number in $i$-th line represents the cost of route from $i$ to $j$ if $i \neq j$, and is 0 otherwise (there are no routes $i \to i$). All route costs are integers from $0$ to $10^8$.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— total cost of the cheapest Masha's successful journey.</p></div>

## Input

<p>First line of input had two integer numbers $n,k$ ($2 \leq n \leq 80; 2 \leq k \leq 10$): number of cities in the country and number of routes in Masha's journey. It is guaranteed that $k$ is even.</p><p>Next $n$ lines hold route descriptions: $j$-th number in $i$-th line represents the cost of route from $i$ to $j$ if $i \neq j$, and is 0 otherwise (there are no routes $i \to i$). All route costs are integers from $0$ to $10^8$.</p>

## Output

<p>Output a single integer&nbsp;— total cost of the cheapest Masha's successful journey.</p>





```input1
5 8
0 1 2 2 0
0 0 1 1 2
0 1 0 0 0
2 1 1 0 0
2 0 1 2 0
```




```input2
3 2
0 1 1
2 0 1
2 2 0
```




```output1
2
```




```output2
3
```


