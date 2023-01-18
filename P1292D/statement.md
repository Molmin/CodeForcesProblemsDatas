## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://soundcloud.com/kivawu/aesir-chaos"><span class="tex-font-style-it">Æsir - CHAOS</span></a></div></div> <div class="epigraph"><div class="epigraph-text"><a href="https://soundcloud.com/kivawu/aesir-v"><span class="tex-font-style-it">Æsir - V.</span></a></div></div><p><span class="tex-font-style-it">"Everything has been planned out. No more hidden concerns. The condition of Cytus is also perfect.</span></p><p><span class="tex-font-style-it">The time right now...... 00:01:12......</span></p><p><span class="tex-font-style-it">It's time."</span></p><p>The emotion samples are now sufficient. After almost 3 years, it's time for Ivy to awake her bonded sister, Vanessa.</p><p>The system inside A.R.C.'s Library core can be considered as an undirected graph with infinite number of processing nodes, numbered with all positive integers ($1, 2, 3, \ldots$). The node with a number $x$ ($x &gt; 1$), is directly connected with a node with number $\frac{x}{f(x)}$, with $f(x)$ being the lowest prime divisor of $x$.</p><p>Vanessa's mind is divided into $n$ fragments. Due to more than 500 years of coma, the fragments have been scattered: the $i$-th fragment is now located at the node with a number $k_i!$ (a factorial of $k_i$).</p><p>To maximize the chance of successful awakening, Ivy decides to place the samples in a node $P$, so that the total length of paths from each fragment to $P$ is smallest possible. If there are multiple fragments located at the same node, the path from that node to $P$ needs to be counted multiple times.</p><p>In the world of zeros and ones, such a requirement is very simple for Ivy. Not longer than a second later, she has already figured out such a node.</p><p>But for a mere human like you, is this still possible?</p><p>For simplicity, please answer the minimal sum of paths' lengths from every fragment to the emotion samples' assembly node $P$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 10^6$)&nbsp;— number of fragments of Vanessa's mind.</p><p>The second line contains $n$ integers: $k_1, k_2, \ldots, k_n$ ($0 \le k_i \le 5000$), denoting the nodes where fragments of Vanessa's mind are located: the $i$-th fragment is at the node with a number $k_i!$.</p></div><div class="output-specification"><p>Print a single integer, denoting the minimal sum of path from every fragment to the node with the emotion samples (a.k.a. node $P$).</p><p>As a reminder, if there are multiple fragments at the same node, the distance from that node to $P$ needs to be counted multiple times as well.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 10^6$)&nbsp;— number of fragments of Vanessa's mind.</p><p>The second line contains $n$ integers: $k_1, k_2, \ldots, k_n$ ($0 \le k_i \le 5000$), denoting the nodes where fragments of Vanessa's mind are located: the $i$-th fragment is at the node with a number $k_i!$.</p>

## Output

<p>Print a single integer, denoting the minimal sum of path from every fragment to the node with the emotion samples (a.k.a. node $P$).</p><p>As a reminder, if there are multiple fragments at the same node, the distance from that node to $P$ needs to be counted multiple times as well.</p>





```input1
3
2 1 4
```




```input2
4
3 1 4 4
```




```input3
4
3 1 4 1
```




```input4
5
3 1 4 1 5
```




```output1
5
```




```output2
6
```




```output3
6
```




```output4
11
```



## Note

<p>Considering the first $24$ nodes of the system, the node network will look as follows (the nodes $1!$, $2!$, $3!$, $4!$ are drawn bold):</p><p><img class="tex-graphics" src="file://jMwJ29zL.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>For the first example, Ivy will place the emotion samples at the node $1$. From here:</p><ul> <li> The distance from Vanessa's first fragment to the node $1$ is $1$. </li><li> The distance from Vanessa's second fragment to the node $1$ is $0$. </li><li> The distance from Vanessa's third fragment to the node $1$ is $4$. </li></ul><p>The total length is $5$.</p><p>For the second example, the assembly node will be $6$. From here:</p><ul> <li> The distance from Vanessa's first fragment to the node $6$ is $0$. </li><li> The distance from Vanessa's second fragment to the node $6$ is $2$. </li><li> The distance from Vanessa's third fragment to the node $6$ is $2$. </li><li> The distance from Vanessa's fourth fragment to the node $6$ is again $2$. </li></ul><p>The total path length is $6$.</p>
