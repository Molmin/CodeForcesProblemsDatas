## Description

<div><p><span class="tex-font-style-bf">It is the hard version of the problem. The difference is that in this version, there are nodes with already chosen colors.</span></p><p>Theofanis is starving, and he wants to eat his favorite food, sheftalia. However, he should first finish his homework. Can you help him with this problem?</p><p>You have a <span class="tex-font-style-it">perfect</span> binary tree of $2^k - 1$ nodes&nbsp;— a binary tree where all vertices $i$ from $1$ to $2^{k - 1} - 1$ have exactly two children: vertices $2i$ and $2i + 1$. Vertices from $2^{k - 1}$ to $2^k - 1$ don't have any children. You want to color its vertices with the $6$ Rubik's cube colors (White, Green, Red, Blue, Orange and Yellow).</p><p>Let's call a coloring <span class="tex-font-style-it">good</span> when all edges connect nodes with colors that are <span class="tex-font-style-it">neighboring</span> sides in the Rubik's cube.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://pVhGPVQs.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://W2lEKx04.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> <span class="tex-font-size-small">A picture of Rubik's cube and its 2D map.</span> </center><p>More formally: </p><ul> <li> a white node can <span class="tex-font-style-bf">not</span> be neighboring with white and yellow nodes; </li><li> a yellow node can <span class="tex-font-style-bf">not</span> be neighboring with white and yellow nodes; </li><li> a green node can <span class="tex-font-style-bf">not</span> be neighboring with green and blue nodes; </li><li> a blue node can <span class="tex-font-style-bf">not</span> be neighboring with green and blue nodes; </li><li> a red node can <span class="tex-font-style-bf">not</span> be neighboring with red and orange nodes; </li><li> an orange node can <span class="tex-font-style-bf">not</span> be neighboring with red and orange nodes; </li></ul><p>However, there are $n$ special nodes in the tree, colors of which are already chosen.</p><p>You want to calculate the number of the good colorings of the binary tree. Two colorings are considered different if at least one node is colored with a different color.</p><p>The answer may be too large, so output the answer modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains the integers $k$ ($1 \le k \le 60$)&nbsp;— the number of levels in the perfect binary tree you need to color.</p><p>The second line contains the integer $n$ ($1 \le n \le \min(2^k - 1, 2000)$)&nbsp;— the number of nodes, colors of which are already chosen.</p><p>The next $n$ lines contains integer $v$ ($1 \le v \le 2^k - 1$) and string $s$&nbsp;— the index of the node and the color of the node ($s$ is one of the <span class="tex-font-style-tt">white</span>, <span class="tex-font-style-tt">yellow</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">red</span> and <span class="tex-font-style-tt">orange</span>).</p><p>It is guaranteed that each node $v$ appears in the input at most once.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of the different colorings modulo $10^9+7$.</p></div>

## Input

<p>The first line contains the integers $k$ ($1 \le k \le 60$)&nbsp;— the number of levels in the perfect binary tree you need to color.</p><p>The second line contains the integer $n$ ($1 \le n \le \min(2^k - 1, 2000)$)&nbsp;— the number of nodes, colors of which are already chosen.</p><p>The next $n$ lines contains integer $v$ ($1 \le v \le 2^k - 1$) and string $s$&nbsp;— the index of the node and the color of the node ($s$ is one of the <span class="tex-font-style-tt">white</span>, <span class="tex-font-style-tt">yellow</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">red</span> and <span class="tex-font-style-tt">orange</span>).</p><p>It is guaranteed that each node $v$ appears in the input at most once.</p>

## Output

<p>Print one integer&nbsp;— the number of the different colorings modulo $10^9+7$.</p>





```input1
3
2
5 orange
2 white
```




```input2
2
2
1 white
2 white
```




```input3
10
3
1 blue
4 red
5 orange
```




```output1
1024
```




```output2
0
```




```output3
328925088
```



## Note

<p>In the picture below, you can see one of the correct colorings of the first test example.</p><center> <img class="tex-graphics" src="file://SEtOObkh.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
