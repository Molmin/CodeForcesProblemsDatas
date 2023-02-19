## Description

<div><p>In Fire City, there are $n$ intersections and $m$ one-way roads. The $i$-th road goes from intersection $a_i$ to $b_i$ and has length $l_i$ miles. </p><p>There are $q$ cars that may only drive along those roads. The $i$-th car starts at intersection $v_i$ and has an odometer that begins at $s_i$, increments for each mile driven, and resets to $0$ whenever it reaches $t_i$. Phoenix has been tasked to drive cars along some roads (possibly none) and <span class="tex-font-style-bf">return them to their initial intersection</span> with the odometer showing $0$.</p><p>For each car, please find if this is possible. </p><p>A car may visit the same road or intersection an arbitrary number of times. The odometers don't stop counting the distance after resetting, so odometers may also be reset an arbitrary number of times.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$; $1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of intersections and the number of roads, respectively.</p><p>Each of the next $m$ lines contain three integers $a_i$, $b_i$, and $l_i$ ($1 \le a_i, b_i \le n$; $a_i \neq b_i$; $1 \le l_i \le 10^9$)&nbsp;— the information about the $i$-th road. The graph is not necessarily connected. It is guaranteed that between any two intersections, there is at most one road for each direction.</p><p>The next line contains an integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of cars.</p><p>Each of the next $q$ lines contains three integers $v_i$, $s_i$, and $t_i$ ($1 \le v_i \le n$; $0 \le s_i &lt; t_i \le 10^9$)&nbsp;— the initial intersection of the $i$-th car, the initial number on the $i$-th odometer, and the number at which the $i$-th odometer resets, respectively.</p></div><div class="output-specification"><p>Print $q$ answers. If the $i$-th car's odometer may be reset to $0$ by driving through some roads (possibly none) and returning to its starting intersection $v_i$, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$; $1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of intersections and the number of roads, respectively.</p><p>Each of the next $m$ lines contain three integers $a_i$, $b_i$, and $l_i$ ($1 \le a_i, b_i \le n$; $a_i \neq b_i$; $1 \le l_i \le 10^9$)&nbsp;— the information about the $i$-th road. The graph is not necessarily connected. It is guaranteed that between any two intersections, there is at most one road for each direction.</p><p>The next line contains an integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of cars.</p><p>Each of the next $q$ lines contains three integers $v_i$, $s_i$, and $t_i$ ($1 \le v_i \le n$; $0 \le s_i &lt; t_i \le 10^9$)&nbsp;— the initial intersection of the $i$-th car, the initial number on the $i$-th odometer, and the number at which the $i$-th odometer resets, respectively.</p>

## Output

<p>Print $q$ answers. If the $i$-th car's odometer may be reset to $0$ by driving through some roads (possibly none) and returning to its starting intersection $v_i$, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
4 4
1 2 1
2 3 1
3 1 2
1 4 3
3
1 1 3
1 2 4
4 0 1
```




```input2
4 5
1 2 1
2 3 1
3 1 2
1 4 1
4 3 2
2
1 2 4
4 3 5
```




```output1
YES
NO
YES
```




```output2
YES
YES
```



## Note

<p>The illustration for the first example is below:</p><center> <img class="tex-graphics" height="265px" src="file://v5oL9tEu.png" style="max-width: 100.0%;max-height: 100.0%;" width="416px">   </center><p>In the first query, Phoenix can drive through the following cities: $1$ $\rightarrow$ $2$ $\rightarrow$ $3$ $\rightarrow$ $1$ $\rightarrow$ $2$ $\rightarrow$ $3$ $\rightarrow$ $1$. The odometer will have reset $3$ times, but it displays $0$ at the end.</p><p>In the second query, we can show that there is no way to reset the odometer to $0$ and return to intersection $1$.</p><p>In the third query, the odometer already displays $0$, so there is no need to drive through any roads.</p><p>Below is the illustration for the second example: </p><center> <img class="tex-graphics" height="265px" src="file://d45grnBP.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px">   </center>
