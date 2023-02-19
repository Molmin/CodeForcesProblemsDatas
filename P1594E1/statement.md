## Description

<div><p><span class="tex-font-style-bf">It is the easy version of the problem. The difference is that in this version, there are no nodes with already chosen colors.</span></p><p>Theofanis is starving, and he wants to eat his favorite food, sheftalia. However, he should first finish his homework. Can you help him with this problem?</p><p>You have a <span class="tex-font-style-it">perfect</span> binary tree of $2^k - 1$ nodes&nbsp;— a binary tree where all vertices $i$ from $1$ to $2^{k - 1} - 1$ have exactly two children: vertices $2i$ and $2i + 1$. Vertices from $2^{k - 1}$ to $2^k - 1$ don't have any children. You want to color its vertices with the $6$ Rubik's cube colors (White, Green, Red, Blue, Orange and Yellow).</p><p>Let's call a coloring <span class="tex-font-style-it">good</span> when all edges connect nodes with colors that are <span class="tex-font-style-it">neighboring</span> sides in the Rubik's cube.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://1F5azY13.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://W2pADA8e.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> <span class="tex-font-size-small">A picture of Rubik's cube and its 2D map.</span> </center><p>More formally: </p><ul> <li> a white node can <span class="tex-font-style-bf">not</span> be neighboring with white and yellow nodes; </li><li> a yellow node can <span class="tex-font-style-bf">not</span> be neighboring with white and yellow nodes; </li><li> a green node can <span class="tex-font-style-bf">not</span> be neighboring with green and blue nodes; </li><li> a blue node can <span class="tex-font-style-bf">not</span> be neighboring with green and blue nodes; </li><li> a red node can <span class="tex-font-style-bf">not</span> be neighboring with red and orange nodes; </li><li> an orange node can <span class="tex-font-style-bf">not</span> be neighboring with red and orange nodes; </li></ul><p>You want to calculate the number of the good colorings of the binary tree. Two colorings are considered different if at least one node is colored with a different color.</p><p>The answer may be too large, so output the answer modulo $10^9+7$.</p></div><div class="input-specification"><p>The first and only line contains the integers $k$ ($1 \le k \le 60$)&nbsp;— the number of levels in the perfect binary tree you need to color.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of the different colorings modulo $10^9+7$.</p></div>

## Input

<p>The first and only line contains the integers $k$ ($1 \le k \le 60$)&nbsp;— the number of levels in the perfect binary tree you need to color.</p>

## Output

<p>Print one integer&nbsp;— the number of the different colorings modulo $10^9+7$.</p>





```input1
3
```




```input2
14
```




```output1
24576
```




```output2
934234
```



## Note

<p>In the picture below, you can see one of the correct colorings of the first example.</p><center> <img class="tex-graphics" src="file://IYRc10C7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
