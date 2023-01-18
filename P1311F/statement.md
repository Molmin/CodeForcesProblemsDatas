## Description

<div><p>There are $n$ points on a coordinate axis $OX$. The $i$-th point is located at the integer point $x_i$ and has a speed $v_i$. It is guaranteed that no two points occupy the same coordinate. All $n$ points move with the constant speed, the coordinate of the $i$-th point at the moment $t$ ($t$ <span class="tex-font-style-bf">can be non-integer</span>) is calculated as $x_i + t \cdot v_i$.</p><p>Consider two points $i$ and $j$. Let $d(i, j)$ be the minimum possible distance between these two points over any possible moments of time (even <span class="tex-font-style-bf">non-integer</span>). It means that if two points $i$ and $j$ coincide at some moment, the value $d(i, j)$ will be $0$.</p><p>Your task is to calculate the value $\sum\limits_{1 \le i &lt; j \le n}$ $d(i, j)$ (the sum of minimum distances over all pairs of points).</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of points.</p><p>The second line of the input contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_i \le 10^8$), where $x_i$ is the initial coordinate of the $i$-th point. It is guaranteed that all $x_i$ are distinct.</p><p>The third line of the input contains $n$ integers $v_1, v_2, \dots, v_n$ ($-10^8 \le v_i \le 10^8$), where $v_i$ is the speed of the $i$-th point.</p></div><div class="output-specification"><p>Print one integer — the value $\sum\limits_{1 \le i &lt; j \le n}$ $d(i, j)$ (the sum of minimum distances over all pairs of points).</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of points.</p><p>The second line of the input contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_i \le 10^8$), where $x_i$ is the initial coordinate of the $i$-th point. It is guaranteed that all $x_i$ are distinct.</p><p>The third line of the input contains $n$ integers $v_1, v_2, \dots, v_n$ ($-10^8 \le v_i \le 10^8$), where $v_i$ is the speed of the $i$-th point.</p>

## Output

<p>Print one integer — the value $\sum\limits_{1 \le i &lt; j \le n}$ $d(i, j)$ (the sum of minimum distances over all pairs of points).</p>





```input1
3
1 3 2
-100 2 3
```




```input2
5
2 1 4 3 5
2 2 2 3 4
```




```input3
2
2 1
-3 0
```




```output1
3
```




```output2
19
```




```output3
0
```


