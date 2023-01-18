## Description

<div><p>Vasya wants to buy himself a nice new car. Unfortunately, he lacks some money. Currently he has exactly <span class="tex-font-style-tt">0</span> burles.</p><p>However, the local bank has $n$ credit offers. Each offer can be described with three numbers $a_i$, $b_i$ and $k_i$. Offers are numbered from $1$ to $n$. If Vasya takes the $i$-th offer, then the bank gives him $a_i$ burles at the beginning of the month and then Vasya pays bank $b_i$ burles at the end of each month for the next $k_i$ months (including the month he activated the offer). <span class="tex-font-style-bf">Vasya can take the offers any order he wants</span>.</p><p><span class="tex-font-style-bf">Each month Vasya can take no more than one credit offer</span>. <span class="tex-font-style-bf">Also each credit offer can not be used more than once</span>. Several credits can be active at the same time. It implies that Vasya pays bank the sum of $b_i$ over all the $i$ of active credits at the end of each month.</p><p>Vasya wants to buy a car in the middle of some month. He just takes all the money he currently has and buys the car of that exact price.</p><p>Vasya don't really care what he'll have to pay the bank back after he buys a car. He just goes out of the country on his car so that the bank can't find him anymore.</p><p>What is the maximum price that car can have?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 500$) — the number of credit offers.</p><p>Each of the next $n$ lines contains three integers $a_i$, $b_i$ and $k_i$ ($1 \le a_i, b_i, k_i \le 10^9$).</p></div><div class="output-specification"><p>Print one integer — the maximum price of the car.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 500$) — the number of credit offers.</p><p>Each of the next $n$ lines contains three integers $a_i$, $b_i$ and $k_i$ ($1 \le a_i, b_i, k_i \le 10^9$).</p>

## Output

<p>Print one integer — the maximum price of the car.</p>





```input1
4
10 9 2
20 33 1
30 115 1
5 3 2
```




```input2
3
40 1 2
1000 1100 5
300 2 1
```




```output1
32
```




```output2
1337
```



## Note

<p>In the first example, the following sequence of offers taken is optimal: <span class="tex-font-style-tt">4</span> $\rightarrow$ <span class="tex-font-style-tt">3</span>.</p><p>The amount of burles Vasya has changes the following way: <span class="tex-font-style-tt">5</span> $\rightarrow$ <span class="tex-font-style-tt">32</span> $\rightarrow$ <span class="tex-font-style-tt">-86</span> $\rightarrow$ .... He takes the money he has in the middle of the second month (<span class="tex-font-style-tt">32</span> burles) and buys the car.</p><p>The negative amount of money means that Vasya has to pay the bank that amount of burles.</p><p>In the second example, the following sequence of offers taken is optimal: <span class="tex-font-style-tt">3</span> $\rightarrow$ <span class="tex-font-style-tt">1</span> $\rightarrow$ <span class="tex-font-style-tt">2</span>.</p><p>The amount of burles Vasya has changes the following way: <span class="tex-font-style-tt">0</span> $\rightarrow$ <span class="tex-font-style-tt">300</span> $\rightarrow$ <span class="tex-font-style-tt">338</span> $\rightarrow$ <span class="tex-font-style-tt">1337</span> $\rightarrow$ <span class="tex-font-style-tt">236</span> $\rightarrow$ <span class="tex-font-style-tt">-866</span> $\rightarrow$ .... </p>
