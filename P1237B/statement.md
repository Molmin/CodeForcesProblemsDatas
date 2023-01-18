## Description

<div><p>Consider a tunnel on a one-way road. During a particular day, $n$ cars numbered from $1$ to $n$ entered and exited the tunnel exactly once. All the cars passed through the tunnel at constant speeds.</p><p>A traffic enforcement camera is mounted at the tunnel entrance. Another traffic enforcement camera is mounted at the tunnel exit. <span class="tex-font-style-it">Perfectly balanced</span>.</p><p>Thanks to the cameras, the order in which the cars entered and exited the tunnel is known. No two cars entered or exited at the same time.</p><p>Traffic regulations prohibit overtaking inside the tunnel. If car $i$ overtakes any other car $j$ inside the tunnel, car $i$ must be fined. However, each car can be fined at most once.</p><p>Formally, let's say that car $i$ <span class="tex-font-style-it">definitely overtook</span> car $j$ if car $i$ entered the tunnel later than car $j$ and exited the tunnel earlier than car $j$. Then, car $i$ must be fined if and only if it definitely overtook at least one other car.</p><p>Find the number of cars that must be fined. </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^5$), denoting the number of cars.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$), denoting the ids of cars in order of entering the tunnel. All $a_i$ are pairwise distinct.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$), denoting the ids of cars in order of exiting the tunnel. All $b_i$ are pairwise distinct.</p></div><div class="output-specification"><p>Output the number of cars to be fined.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^5$), denoting the number of cars.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$), denoting the ids of cars in order of entering the tunnel. All $a_i$ are pairwise distinct.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$), denoting the ids of cars in order of exiting the tunnel. All $b_i$ are pairwise distinct.</p>

## Output

<p>Output the number of cars to be fined.</p>





```input1
5
3 5 2 1 4
4 3 2 5 1
```




```input2
7
5 2 3 6 7 1 4
2 3 6 7 1 4 5
```




```input3
2
1 2
1 2
```




```output1
2
```




```output2
6
```




```output3
0
```



## Note

<p>The first example is depicted below:</p><p><img class="tex-graphics" src="file://H65OcJn6.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Car $2$ definitely overtook car $5$, while car $4$ definitely overtook cars $1$, $2$, $3$ and $5$. Cars $2$ and $4$ must be fined.</p><p>In the second example car $5$ was definitely overtaken by all other cars.</p><p>In the third example no car must be fined.</p>
