## Description

<div><p>In Byteland, there are two political parties fighting for seats in the Parliament in the upcoming elections: <span class="tex-font-style-it">Wrong Answer Party</span> and <span class="tex-font-style-it">Time Limit Exceeded Party</span>. As they want to convince as many citizens as possible to cast their votes on them, they keep promising lower and lower taxes.</p><p>There are $n$ cities in Byteland, connected by $m$ one-way roads. Interestingly enough, the road network has no cycles — it's impossible to start in any city, follow a number of roads, and return to that city. Last year, citizens of the $i$-th city had to pay $h_i$ bourles of tax.</p><p>Parties will now alternately hold the election conventions in various cities. If a party holds a convention in city $v$, the party needs to <span class="tex-font-style-it">decrease</span> the taxes in this city to a non-negative integer amount of bourles. However, at the same time they can arbitrarily modify the taxes in each of the cities that can be reached from $v$ using a single road. The only condition that must be fulfilled that the tax in each city has to remain a non-negative integer amount of bourles.</p><p>The first party to hold the convention is <span class="tex-font-style-it">Wrong Answer Party</span>. It's predicted that the party to hold the last convention will win the election. Can <span class="tex-font-style-it">Wrong Answer Party</span> win regardless of <span class="tex-font-style-it">Time Limit Exceeded Party</span>'s moves?</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$, $m$ ($1 \leq n \leq 200\,000$, $0 \leq m \leq 200\,000$) — the number of cities and roads in Byteland.</p><p>The next line contains $n$ space-separated integers $h_1, h_2, \dots, h_n$ ($0 \leq h_i \leq 10^9$); $h_i$ denotes the amount of taxes paid in the $i$-th city.</p><p>Each of the following $m$ lines contains two integers ($1 \leq u, v \leq n$, $u \neq v$), and describes a one-way road leading from the city $u$ to the city $v$. There will be no cycles in the road network. No two roads will connect the same pair of cities.</p><p>We can show that the conventions cannot be held indefinitely for any correct test case.</p></div><div class="output-specification"><p>If <span class="tex-font-style-it">Wrong Answer Party</span> can win the election, output <span class="tex-font-style-tt">WIN</span> in the first line of your output. In this case, you're additionally asked to produce any convention allowing the party to win regardless of the opponent's actions. The second line should contain $n$ non-negative integers $h'_1, h'_2, \dots, h'_n$ ($0 \leq h'_i \leq 2 \cdot 10^{18}$) describing the amount of taxes paid in consecutive cities after the convention. If there are multiple answers, output any. We guarantee that if the party has any winning move, there exists a move after which no city has to pay more than $2 \cdot 10^{18}$ bourles.</p><p>If the party cannot assure their victory, output <span class="tex-font-style-tt">LOSE</span> in the first and only line of the output.</p></div>

## Input

<p>The first line of the input contains two integers $n$, $m$ ($1 \leq n \leq 200\,000$, $0 \leq m \leq 200\,000$) — the number of cities and roads in Byteland.</p><p>The next line contains $n$ space-separated integers $h_1, h_2, \dots, h_n$ ($0 \leq h_i \leq 10^9$); $h_i$ denotes the amount of taxes paid in the $i$-th city.</p><p>Each of the following $m$ lines contains two integers ($1 \leq u, v \leq n$, $u \neq v$), and describes a one-way road leading from the city $u$ to the city $v$. There will be no cycles in the road network. No two roads will connect the same pair of cities.</p><p>We can show that the conventions cannot be held indefinitely for any correct test case.</p>

## Output

<p>If <span class="tex-font-style-it">Wrong Answer Party</span> can win the election, output <span class="tex-font-style-tt">WIN</span> in the first line of your output. In this case, you're additionally asked to produce any convention allowing the party to win regardless of the opponent's actions. The second line should contain $n$ non-negative integers $h'_1, h'_2, \dots, h'_n$ ($0 \leq h'_i \leq 2 \cdot 10^{18}$) describing the amount of taxes paid in consecutive cities after the convention. If there are multiple answers, output any. We guarantee that if the party has any winning move, there exists a move after which no city has to pay more than $2 \cdot 10^{18}$ bourles.</p><p>If the party cannot assure their victory, output <span class="tex-font-style-tt">LOSE</span> in the first and only line of the output.</p>





```input1
4 2
2 1 1 5
1 2
3 4
```




```input2
4 2
1 5 1 5
1 2
3 4
```




```input3
3 3
314 159 265
1 2
1 3
3 2
```




```input4
6 4
2 2 5 5 6 6
1 3
2 4
3 5
4 6
```




```output1
WIN
1 5 1 5
```




```output2
LOSE
```




```output3
WIN
0 0 0
```




```output4
LOSE
```



## Note

<p>In the first example, <span class="tex-font-style-it">Wrong Answer Party</span> should hold the convention in the city $1$. The party will decrease the taxes in this city to $1$ bourle. As the city $2$ is directly reachable from $1$, we can arbitrarily modify the taxes in this city. The party should change the tax to $5$ bourles. It can be easily proved that <span class="tex-font-style-it">Time Limit Exceeded</span> cannot win the election after this move if <span class="tex-font-style-it">Wrong Answer Party</span> plays optimally.</p><p>The second example test presents the situation we created after a single move in the previous test; as it's <span class="tex-font-style-it">Wrong Answer Party</span>'s move now, the party cannot win.</p><p>In the third test, we should hold the convention in the first city. This allows us to change the taxes in any city to any desired value; we can for instance decide to set all the taxes to zero, which allows the <span class="tex-font-style-it">Wrong Answer Party</span> to win the election immediately.</p>
