## Description

<div><p>In a magical land there are $n$ cities conveniently numbered $1, 2, \dots, n$. Some pairs of these cities are connected by magical colored roads. Magic is unstable, so at any time, new roads may appear between two cities.</p><p>Vicky the witch has been tasked with performing deliveries between some pairs of cities. However, Vicky is a beginner, so she can only complete a delivery if she can move from her starting city to her destination city through a <span class="tex-font-style-it">double rainbow</span>. A double rainbow is a sequence of cities $c_1, c_2, \dots, c_k$ satisfying the following properties:</p><ul> <li> For each $i$ with $1 \le i \le k - 1$, the cities $c_i$ and $c_{i + 1}$ are connected by a road. </li><li> For each $i$ with $1 \le i \le \frac{k - 1}{2}$, the roads connecting $c_{2i}$ with $c_{2i - 1}$ and $c_{2i + 1}$ have the same color. </li></ul><p>For example if $k = 5$, the road between $c_1$ and $c_2$ must be the same color as the road between $c_2$ and $c_3$, and the road between $c_3$ and $c_4$ must be the same color as the road between $c_4$ and $c_5$.</p><p>Vicky has a list of events in chronological order, where each event is either a delivery she must perform, or appearance of a new road. Help her determine which of her deliveries she will be able to complete.</p></div><div class="input-specification"><p>The first line contains four integers $n$, $m$, $c$, and $q$ ($2 \le n \le 10^5$, $1 \le m, c, q \le 10^5$), denoting respectively the number of cities, the number of roads initially present, the number of different colors the roads can take, and the number of events.</p><p>Each of the following $m$ lines contains three integers $x$, $y$, and $z$ ($1 \le x, y \le n$, $1 \le z \le c$), describing that there initially exists a bidirectional road with color $z$ between cities $x$ and $y$.</p><p>Then $q$ lines follow, describing the events. Each event is one of the following two types: </p><ol> <li> <span class="tex-font-style-tt">+ x y z</span> ($1 \le x, y \le n$, $1 \le z \le c$), meaning a road with color $z$ appears between cities $x$ and $y$; </li><li> <span class="tex-font-style-tt">? x y</span> ($1 \le x, y \le n$), meaning you should determine whether Vicky can make a delivery starting at city $x$ and ending at city $y$. It is guaranteed that $x \neq y$. </li></ol><p>It is guaranteed that at any moment, there is at most one road connecting any pair of cities, and that no road connects a city to itself. It is guaranteed that the input contains at least one event of the second type.</p></div><div class="output-specification"><p>For each event of the second type, print a single line containing "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the delivery can be made, or a single line containing "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line contains four integers $n$, $m$, $c$, and $q$ ($2 \le n \le 10^5$, $1 \le m, c, q \le 10^5$), denoting respectively the number of cities, the number of roads initially present, the number of different colors the roads can take, and the number of events.</p><p>Each of the following $m$ lines contains three integers $x$, $y$, and $z$ ($1 \le x, y \le n$, $1 \le z \le c$), describing that there initially exists a bidirectional road with color $z$ between cities $x$ and $y$.</p><p>Then $q$ lines follow, describing the events. Each event is one of the following two types: </p><ol> <li> <span class="tex-font-style-tt">+ x y z</span> ($1 \le x, y \le n$, $1 \le z \le c$), meaning a road with color $z$ appears between cities $x$ and $y$; </li><li> <span class="tex-font-style-tt">? x y</span> ($1 \le x, y \le n$), meaning you should determine whether Vicky can make a delivery starting at city $x$ and ending at city $y$. It is guaranteed that $x \neq y$. </li></ol><p>It is guaranteed that at any moment, there is at most one road connecting any pair of cities, and that no road connects a city to itself. It is guaranteed that the input contains at least one event of the second type.</p>

## Output

<p>For each event of the second type, print a single line containing "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the delivery can be made, or a single line containing "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p>





```input1
4 3 2 4
1 2 1
2 3 1
3 4 2
? 1 4
? 4 1
+ 3 1 2
? 4 1
```




```output1
Yes
No
Yes
```



## Note

<p>The following picture corresponds to the sample.</p><center> <img class="tex-graphics" src="file://latc212f.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For her first delivery, Vicky can use the sequence <span class="tex-font-style-tt">1, 2, 3, 4</span> which is a double rainbow. However, she cannot complete the second delivery, as she can only reach city $3$. After adding the road between cities $1$ and $3$, she can now complete a delivery from city $4$ to city $1$ by using the double rainbow <span class="tex-font-style-tt">4, 3, 1</span>.</p>
