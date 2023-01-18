## Description

<div><p>Farmer John is obsessed with making Bessie exercise more!</p><p>Bessie is out grazing on the farm, which consists of $n$ fields connected by $m$ directed roads. Each road takes some time $w_i$ to cross. She is currently at field $1$ and will return to her home at field $n$ at the end of the day.</p><p>Farmer John has plans to increase the time it takes to cross certain roads. He can increase the time it takes to cross each road by a nonnegative amount, but the total increase cannot exceed $x_i$ for the $i$-th plan. </p><p>Determine the maximum he can make the shortest path from $1$ to $n$ for each of the $q$ independent plans.</p></div><div class="input-specification"><p>The first line contains integers $n$ and $m$ ($2 \le n \le 50$, $1 \le m \le n \cdot (n-1)$) — the number of fields and number of roads, respectively.</p><p>Each of the following $m$ lines contains $3$ integers, $u_i$, $v_i$, and $w_i$ ($1 \le u_i, v_i \le n$, $1 \le w_i \le 10^6$), meaning there is an road from field $u_i$ to field $v_i$ that takes $w_i$ time to cross.</p><p>It is guaranteed that there exists a way to get to field $n$ from field $1$. It is guaranteed that the graph does not contain self-loops or parallel edges. It is possible to have a road from $u$ to $v$ and a road from $v$ to $u$.</p><p>The next line contains a single integer $q$ ($1 \le q \le 10^5$), the number of plans.</p><p>Each of the following $q$ lines contains a single integer $x_i$, the query ($0 \le x_i \le 10^5$).</p></div><div class="output-specification"><p>For each query, output the maximum Farmer John can make the shortest path if the total increase does not exceed $x_i$.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-6}$.</p></div>

## Input

<p>The first line contains integers $n$ and $m$ ($2 \le n \le 50$, $1 \le m \le n \cdot (n-1)$) — the number of fields and number of roads, respectively.</p><p>Each of the following $m$ lines contains $3$ integers, $u_i$, $v_i$, and $w_i$ ($1 \le u_i, v_i \le n$, $1 \le w_i \le 10^6$), meaning there is an road from field $u_i$ to field $v_i$ that takes $w_i$ time to cross.</p><p>It is guaranteed that there exists a way to get to field $n$ from field $1$. It is guaranteed that the graph does not contain self-loops or parallel edges. It is possible to have a road from $u$ to $v$ and a road from $v$ to $u$.</p><p>The next line contains a single integer $q$ ($1 \le q \le 10^5$), the number of plans.</p><p>Each of the following $q$ lines contains a single integer $x_i$, the query ($0 \le x_i \le 10^5$).</p>

## Output

<p>For each query, output the maximum Farmer John can make the shortest path if the total increase does not exceed $x_i$.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-6}$.</p>





```input1
3 3
1 2 2
2 3 2
1 3 3
5
0
1
2
3
4
```




```output1
3.0000000000
4.0000000000
4.5000000000
5.0000000000
5.5000000000
```


