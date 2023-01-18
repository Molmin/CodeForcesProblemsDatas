## Description

<div><p>Several days ago you bought a new house and now you are planning to start a renovation. Since winters in your region can be very cold you need to decide how to heat rooms in your house.</p><p>Your house has $n$ rooms. In the $i$-th room you can install at most $c_i$ heating radiators. Each radiator can have several sections, but the cost of the radiator with $k$ sections is equal to $k^2$ burles.</p><p>Since rooms can have different sizes, you calculated that you need at least $sum_i$ sections in total in the $i$-th room. </p><p>For each room calculate the minimum cost to install at most $c_i$ radiators with total number of sections not less than $sum_i$.</p></div><div class="input-specification"><p>The first line contains single integer $n$ ($1 \le n \le 1000$) — the number of rooms.</p><p>Each of the next $n$ lines contains the description of some room. The $i$-th line contains two integers $c_i$ and $sum_i$ ($1 \le c_i, sum_i \le 10^4$) — the maximum number of radiators and the minimum total number of sections in the $i$-th room, respectively.</p></div><div class="output-specification"><p>For each room print one integer — the minimum possible cost to install at most $c_i$ radiators with total number of sections not less than $sum_i$.</p></div>

## Input

<p>The first line contains single integer $n$ ($1 \le n \le 1000$) — the number of rooms.</p><p>Each of the next $n$ lines contains the description of some room. The $i$-th line contains two integers $c_i$ and $sum_i$ ($1 \le c_i, sum_i \le 10^4$) — the maximum number of radiators and the minimum total number of sections in the $i$-th room, respectively.</p>

## Output

<p>For each room print one integer — the minimum possible cost to install at most $c_i$ radiators with total number of sections not less than $sum_i$.</p>





```input1
4
1 10000
10000 1
2 6
4 6
```




```output1
100000000
1
18
10
```



## Note

<p>In the first room, you can install only one radiator, so it's optimal to use the radiator with $sum_1$ sections. The cost of the radiator is equal to $(10^4)^2 = 10^8$.</p><p>In the second room, you can install up to $10^4$ radiators, but since you need only one section in total, it's optimal to buy one radiator with one section.</p><p>In the third room, there $7$ variants to install radiators: $[6, 0]$, $[5, 1]$, $[4, 2]$, $[3, 3]$, $[2, 4]$, $[1, 5]$, $[0, 6]$. The optimal variant is $[3, 3]$ and it costs $3^2+ 3^2 = 18$.</p>
