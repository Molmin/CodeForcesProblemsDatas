## Description

<div><p>Shichikuji is the new resident deity of the South Black Snail Temple. Her first job is as follows:</p><p>There are $n$ new cities located in Prefecture X. Cities are numbered from $1$ to $n$. City $i$ is located $x_i$ km North of the shrine and $y_i$ km East of the shrine. It is possible that $(x_i, y_i) = (x_j, y_j)$ even when $i \ne j$.</p><p>Shichikuji must provide electricity to each city either by building a power station in that city, or by making a connection between that city and another one that already has electricity. So the City has electricity if it has a power station in it or it is connected to a City which has electricity by a direct connection or via a chain of connections.</p><ul>  <li>   Building a power station in City $i$ will cost $c_i$ yen;  </li><li>   Making a connection between City $i$ and City $j$ will cost $k_i + k_j$ yen <span class="tex-font-style-bf">per km of wire</span> used for the connection. However, wires can only go the cardinal directions (North, South, East, West). Wires can cross each other. Each wire must have both of its endpoints in some cities. If City $i$ and City $j$ are connected by a wire, the wire will go through any shortest path from City $i$ to City $j$. Thus, the length of the wire if City $i$ and City $j$ are connected is $|x_i - x_j| + |y_i - y_j|$ km. </li></ul><p>Shichikuji wants to do this job spending as little money as possible, since according to her, there isn't really anything else in the world other than money. However, she died when she was only in fifth grade so she is not smart enough for this. And thus, the new resident deity asks for your help.</p><p>And so, you have to provide Shichikuji with the following information: minimum amount of yen needed to provide electricity to all cities, the cities in which power stations will be built, and the connections to be made.</p><p>If there are multiple ways to choose the cities and the connections to obtain the construction of minimum price, then print any of them.</p></div><div class="input-specification"><p>First line of input contains a single integer $n$ ($1 \leq n \leq 2000$) — the number of cities.</p><p>Then, $n$ lines follow. The $i$-th line contains two space-separated integers $x_i$ ($1 \leq x_i \leq 10^6$) and $y_i$ ($1 \leq y_i \leq 10^6$) — the coordinates of the $i$-th city.</p><p>The next line contains $n$ space-separated integers $c_1, c_2, \dots, c_n$ ($1 \leq c_i \leq 10^9$) — the cost of building a power station in the $i$-th city.</p><p>The last line contains $n$ space-separated integers $k_1, k_2, \dots, k_n$ ($1 \leq k_i \leq 10^9$).</p></div><div class="output-specification"><p>In the first line print a single integer, denoting the minimum amount of yen needed.</p><p>Then, print an integer $v$ — the number of power stations to be built.</p><p>Next, print $v$ space-separated integers, denoting the indices of cities in which a power station will be built. Each number should be from $1$ to $n$ and all numbers should be pairwise distinct. You can print the numbers in arbitrary order.</p><p>After that, print an integer $e$ — the number of connections to be made.</p><p>Finally, print $e$ pairs of integers $a$ and $b$ ($1 \le a, b \le n$, $a \ne b$), denoting that a connection between City $a$ and City $b$ will be made. Each unordered pair of cities should be included at most once (for each $(a, b)$ there should be no more $(a, b)$ or $(b, a)$ pairs). You can print the pairs in arbitrary order.</p><p>If there are multiple ways to choose the cities and the connections to obtain the construction of minimum price, then print any of them.</p></div>

## Input

<p>First line of input contains a single integer $n$ ($1 \leq n \leq 2000$) — the number of cities.</p><p>Then, $n$ lines follow. The $i$-th line contains two space-separated integers $x_i$ ($1 \leq x_i \leq 10^6$) and $y_i$ ($1 \leq y_i \leq 10^6$) — the coordinates of the $i$-th city.</p><p>The next line contains $n$ space-separated integers $c_1, c_2, \dots, c_n$ ($1 \leq c_i \leq 10^9$) — the cost of building a power station in the $i$-th city.</p><p>The last line contains $n$ space-separated integers $k_1, k_2, \dots, k_n$ ($1 \leq k_i \leq 10^9$).</p>

## Output

<p>In the first line print a single integer, denoting the minimum amount of yen needed.</p><p>Then, print an integer $v$ — the number of power stations to be built.</p><p>Next, print $v$ space-separated integers, denoting the indices of cities in which a power station will be built. Each number should be from $1$ to $n$ and all numbers should be pairwise distinct. You can print the numbers in arbitrary order.</p><p>After that, print an integer $e$ — the number of connections to be made.</p><p>Finally, print $e$ pairs of integers $a$ and $b$ ($1 \le a, b \le n$, $a \ne b$), denoting that a connection between City $a$ and City $b$ will be made. Each unordered pair of cities should be included at most once (for each $(a, b)$ there should be no more $(a, b)$ or $(b, a)$ pairs). You can print the pairs in arbitrary order.</p><p>If there are multiple ways to choose the cities and the connections to obtain the construction of minimum price, then print any of them.</p>





```input1
3
2 3
1 1
3 2
3 2 3
3 2 3
```




```input2
3
2 1
1 2
3 3
23 2 23
3 2 3
```




```output1
8
3
1 2 3 
0
```




```output2
27
1
2 
2
1 2
2 3
```



## Note

<p>For the answers given in the samples, refer to the following diagrams (cities with power stations are colored green, other cities are colored blue, and wires are colored red):</p><p><img class="tex-graphics" src="file://rPFGACYf.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>For the first example, the cost of building power stations in all cities is $3 + 2 + 3 = 8$. It can be shown that no configuration costs less than 8 yen.</p><p>For the second example, the cost of building a power station in City 2 is 2. The cost of connecting City 1 and City 2 is $2 \cdot (3 + 2) = 10$. The cost of connecting City 2 and City 3 is $3 \cdot (2 + 3) = 15$. Thus the total cost is $2 + 10 + 15 = 27$. It can be shown that no configuration costs less than 27 yen.</p>
