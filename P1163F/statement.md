## Description

<div><p>In the city of Capypaland where Kuro and Shiro resides, there are $n$ towns numbered from $1$ to $n$ and there are $m$ bidirectional roads numbered from $1$ to $m$ connecting them. The $i$-th road connects towns $u_i$ and $v_i$. Since traveling between the towns is quite difficult, the taxi industry is really popular here. To survive the harsh competition, each taxi company has to find a distinctive trait for their customers.</p><p>Kuro is the owner of a taxi company. He has decided to introduce a new fee model for his taxi brand, where the fee for each ride is not calculated based on the trip length, but on the sum of the prices of the roads traveled. The price for each of the $m$ roads has been decided by Kuro himself.</p><p>As of now, the price for the road $i$ is $w_i$ and hence the fee for a taxi ride traveling through roads $e_1, e_2, \ldots, e_k$ is $\sum_{i=1}^k w_{e_i}$.</p><p>However, Kuro himself is an indecisive person, so he has drafted $q$ plans to change the road price. Each of the plans will be based on the original prices $w_i$, except for a single road $t_j$, the price of which is changed to $x_j$. Note, that the plans are independent of each other.</p><p>Shiro is a regular customer of the Kuro's taxi brand since she uses the taxi to travel from town $1$ to town $n$ every day. Since she's so a regular customer, Kuro decided to show her all his $q$ plans before publishing them to the public. Now, Shiro wants to know the lowest fee she must pay to travel from the town $1$ to the town $n$ for each Kuro's plan.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $q$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m, q \le 2 \cdot 10^5$)&nbsp;— the number of towns, the number of roads, and the number of plans that Kuro has drafted respectively.</p><p>The $i$-th of the next $m$ contains three integers $u_i$, $v_i$ and $w_i$ ($1 \le u_i, v_i \le n$, $1 \le w_i \le 10^9$, $u_i \ne v_i$)&nbsp;— two endpoints and the original price of the $i$-th road.</p><p>It is guaranteed, that there is at least one way to travel from town $1$ to town $n$ using these $m$ bidirectional roads.</p><p>Each of the next $q$ lines contains two integers $t_j$ and $x_j$ ($1 \leq t_j \leq m, 1 \leq x_j \leq 10^9$)&nbsp;— the index of the road Kuro has planned to change and its new price respectively.</p></div><div class="output-specification"><p>Print $q$ integers&nbsp;— the lowest fee Shiro must pay to get from town $1$ to town $n$ in each of those $q$ plans.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $q$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m, q \le 2 \cdot 10^5$)&nbsp;— the number of towns, the number of roads, and the number of plans that Kuro has drafted respectively.</p><p>The $i$-th of the next $m$ contains three integers $u_i$, $v_i$ and $w_i$ ($1 \le u_i, v_i \le n$, $1 \le w_i \le 10^9$, $u_i \ne v_i$)&nbsp;— two endpoints and the original price of the $i$-th road.</p><p>It is guaranteed, that there is at least one way to travel from town $1$ to town $n$ using these $m$ bidirectional roads.</p><p>Each of the next $q$ lines contains two integers $t_j$ and $x_j$ ($1 \leq t_j \leq m, 1 \leq x_j \leq 10^9$)&nbsp;— the index of the road Kuro has planned to change and its new price respectively.</p>

## Output

<p>Print $q$ integers&nbsp;— the lowest fee Shiro must pay to get from town $1$ to town $n$ in each of those $q$ plans.</p>





```input1
4 5 6
1 2 2
2 4 3
1 4 7
1 3 1
3 4 5
3 4
5 1
3 8
1 4
2 1
3 1
```




```input2
2 4 4
1 2 2
1 2 3
1 2 4
1 2 5
2 1
3 2
4 3
1 5
```




```input3
2 1 1
1 2 1
1 3
```




```output1
4
2
5
6
3
1
```




```output2
1
2
2
3
```




```output3
3
```



## Note

<p>In the first example, the original overview of Capypaland looks like this, where the number next to each road denotes the original prices of the roads,</p><center> <img class="tex-graphics" src="file://w8IFbdNb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The overview of the first plan,</p><center> <img class="tex-graphics" src="file://MBfZWE56.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The lowest fee Shiro must pay in this plan is $4$, which corresponds to the path $1 \rightarrow 4$.</p><p>The overview of the second plan,</p><center> <img class="tex-graphics" src="file://WHmcW0d4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The lowest fee Shiro must pay in this plan is $2$, which corresponds to the path $1 \rightarrow 3 \rightarrow 4$.</p><p>The overview of the third plan,</p><center> <img class="tex-graphics" src="file://PjYjbmOk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The lowest fee Shiro must pay in this plan is $5$, which corresponds to the path $1 \rightarrow 2 \rightarrow 4$.</p>
