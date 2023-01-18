## Description

<div><p>There are two types of burgers in your restaurant — hamburgers and chicken burgers! To assemble a hamburger you need two buns and a beef patty. To assemble a chicken burger you need two buns and a chicken cutlet. </p><p>You have $b$ buns, $p$ beef patties and $f$ chicken cutlets in your restaurant. You can sell one hamburger for $h$ dollars and one chicken burger for $c$ dollars. Calculate the maximum profit you can achieve.</p><p>You have to answer $t$ independent queries.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) – the number of queries.</p><p>The first line of each query contains three integers $b$, $p$ and $f$ ($1 \le b, ~p, ~f \le 100$) — the number of buns, beef patties and chicken cutlets in your restaurant.</p><p>The second line of each query contains two integers $h$ and $c$ ($1 \le h, ~c \le 100$) — the hamburger and chicken burger prices in your restaurant.</p></div><div class="output-specification"><p>For each query print one integer — the maximum profit you can achieve.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) – the number of queries.</p><p>The first line of each query contains three integers $b$, $p$ and $f$ ($1 \le b, ~p, ~f \le 100$) — the number of buns, beef patties and chicken cutlets in your restaurant.</p><p>The second line of each query contains two integers $h$ and $c$ ($1 \le h, ~c \le 100$) — the hamburger and chicken burger prices in your restaurant.</p>

## Output

<p>For each query print one integer — the maximum profit you can achieve.</p>





```input1
3
15 2 3
5 10
7 5 2
10 12
1 100 100
100 100
```




```output1
40
34
0
```



## Note

<p>In first query you have to sell two hamburgers and three chicken burgers. Your income is $2 \cdot 5 + 3 \cdot 10 = 40$.</p><p>In second query you have to ell one hamburgers and two chicken burgers. Your income is $1 \cdot 10 + 2 \cdot 12 = 34$.</p><p>In third query you can not create any type of burgers because because you have only one bun. So your income is zero.</p>
