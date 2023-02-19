## Description

<div><p><span class="tex-font-style-it">Lee was planning to get closer to Mashtali's heart to proceed with his evil plan(which we're not aware of, yet), so he decided to beautify Mashtali's graph. But he made several rules for himself. And also he was too busy with his plans that he didn't have time for such minor tasks, so he asked you for help.</span></p><p>Mashtali's graph is an <span class="tex-font-style-bf">undirected</span> weighted graph with $n$ vertices and $m$ edges with weights equal to either $1$ or $2$. Lee wants to direct the edges of Mashtali's graph so that it will be as beautiful as possible.</p><p>Lee thinks that the beauty of a directed weighted graph is equal to the number of its Oddysey vertices. A vertex $v$ is an Oddysey vertex if $|d^+(v) - d^-(v)| = 1$, where $d^+(v)$ is the sum of weights of the outgoing from $v$ edges, and $d^-(v)$ is the sum of the weights of the incoming to $v$ edges.</p><p>Find the largest possible beauty of a graph that Lee can achieve by directing the edges of Mashtali's graph. In addition, find any way to achieve it.</p><p>Note that you have to orient each edge.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ $(1 \le n \le 10^5;\; 1 \le m \le 10^5)$&nbsp;— the numbers of vertices and edges in the graph.</p><p>The $i$-th line of the following $m$ lines contains three integers $u_i$, $v_i$ and $w_i$ $( 1 \le u_i , v_i \le n;\; u_i \neq v_i;\; \bf{w_i \in \{1, 2\}} )$&nbsp;— the endpoints of the $i$-th edge and its weight.</p><p>Note that the graph doesn't have to be connected, and it might contain multiple edges.</p></div><div class="output-specification"><p>In the first line print a single integer&nbsp;— the maximum beauty of the graph Lee can achieve.</p><p>In the second line print a string of length $m$ consisting of $1$s and $2$s&nbsp;— directions of the edges.</p><p>If you decide to direct the $i$-th edge from vertex $u_i$ to vertex $v_i$, $i$-th character of the string should be $1$. Otherwise, it should be $2$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ $(1 \le n \le 10^5;\; 1 \le m \le 10^5)$&nbsp;— the numbers of vertices and edges in the graph.</p><p>The $i$-th line of the following $m$ lines contains three integers $u_i$, $v_i$ and $w_i$ $( 1 \le u_i , v_i \le n;\; u_i \neq v_i;\; \bf{w_i \in \{1, 2\}} )$&nbsp;— the endpoints of the $i$-th edge and its weight.</p><p>Note that the graph doesn't have to be connected, and it might contain multiple edges.</p>

## Output

<p>In the first line print a single integer&nbsp;— the maximum beauty of the graph Lee can achieve.</p><p>In the second line print a string of length $m$ consisting of $1$s and $2$s&nbsp;— directions of the edges.</p><p>If you decide to direct the $i$-th edge from vertex $u_i$ to vertex $v_i$, $i$-th character of the string should be $1$. Otherwise, it should be $2$.</p>





```input1
6 7
1 2 1
1 3 2
2 3 2
1 4 1
4 5 1
2 5 2
2 6 2
```




```input2
6 7
1 2 2
1 3 2
2 3 2
1 4 2
4 5 2
2 5 2
2 6 2
```




```input3
6 7
1 2 1
1 3 1
2 3 1
1 4 1
4 5 1
2 5 1
2 6 1
```




```output1
2
1212212
```




```output2
0
1212212
```




```output3
2
1212212
```



## Note

<p>Explanation for the first sample:</p><center> <img class="tex-graphics" src="file://SSFyByIy.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">vertices $2$ and $5$ are Oddyseys.</span> </center><p>Explanation for the third sample:</p><center> <img class="tex-graphics" src="file://2d5OU7qk.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">vertices $1$ and $6$ are Oddyseys.</span> </center>
