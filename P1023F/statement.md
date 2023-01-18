## Description

<div><p>You are managing a mobile phone network, and want to offer competitive prices to connect a network.</p><p>The network has $n$ nodes.</p><p>Your competitor has already offered some connections between some nodes, with some fixed prices. These connections are bidirectional. There are initially $m$ connections the competitor is offering. The $i$-th connection your competitor is offering will connect nodes $fa_i$ and $fb_i$ and costs $fw_i$. </p><p>You have a list of $k$ connections that you want to offer. It is guaranteed that this set of connection does not form any cycle. The $j$-th of these connections will connect nodes $ga_j$ and $gb_j$. These connections are also bidirectional. The cost of these connections have not been decided yet.</p><p>You can set the prices of these connections to any arbitrary integer value. These prices are set independently for each connection. After setting the prices, the customer will choose such $n - 1$ connections that all nodes are connected in a single network and the total cost of chosen connections is minimum possible. If there are multiple ways to choose such networks, the customer will choose an arbitrary one that also maximizes the number of your connections in it.</p><p>You want to set prices in such a way such that <span class="tex-font-style-bf">all</span> your $k$ connections are chosen by the customer, and the sum of prices of your connections is maximized.</p><p>Print the maximum profit you can achieve, or $-1$ if it is unbounded.</p></div><div class="input-specification"><p>The first line of input will contain three integers $n$, $k$ and $m$ ($1 \leq n, k, m \leq 5 \cdot 10^5, k \leq n-1$), the number of nodes, the number of your connections, and the number of competitor connections, respectively.</p><p>The next $k$ lines contain two integers $ga_i$ and $gb_i$ ($1 \leq ga_i, gb_i \leq n$, $ga_i \not= gb_i$), representing one of your connections between nodes $ga_i$ and $gb_i$. Your set of connections is guaranteed to be acyclic.</p><p>The next $m$ lines contain three integers each, $fa_i$, $fb_i$ and $fw_i$ ($1 \leq fa_i, fb_i \leq n$, $fa_i \not= fb_i$, $1 \leq fw_i \leq 10^9$), denoting one of your competitor's connections between nodes $fa_i$ and $fb_i$ with cost $fw_i$. None of these connections connects a node to itself, and no pair of these connections connect the same pair of nodes. In addition, these connections are given by non-decreasing order of cost (that is, $fw_{i-1} \leq fw_i$ for all valid $i$).</p><p>Note that there may be some connections that appear in both your set and your competitor's set (though no connection will appear twice in one of this sets).</p><p>It is guaranteed that the union of all of your connections and your competitor's connections form a connected network.</p></div><div class="output-specification"><p>Print a single integer, the maximum possible profit you can achieve if you set the prices on your connections appropriately. If the profit is unbounded, print $-1$.</p></div>

## Input

<p>The first line of input will contain three integers $n$, $k$ and $m$ ($1 \leq n, k, m \leq 5 \cdot 10^5, k \leq n-1$), the number of nodes, the number of your connections, and the number of competitor connections, respectively.</p><p>The next $k$ lines contain two integers $ga_i$ and $gb_i$ ($1 \leq ga_i, gb_i \leq n$, $ga_i \not= gb_i$), representing one of your connections between nodes $ga_i$ and $gb_i$. Your set of connections is guaranteed to be acyclic.</p><p>The next $m$ lines contain three integers each, $fa_i$, $fb_i$ and $fw_i$ ($1 \leq fa_i, fb_i \leq n$, $fa_i \not= fb_i$, $1 \leq fw_i \leq 10^9$), denoting one of your competitor's connections between nodes $fa_i$ and $fb_i$ with cost $fw_i$. None of these connections connects a node to itself, and no pair of these connections connect the same pair of nodes. In addition, these connections are given by non-decreasing order of cost (that is, $fw_{i-1} \leq fw_i$ for all valid $i$).</p><p>Note that there may be some connections that appear in both your set and your competitor's set (though no connection will appear twice in one of this sets).</p><p>It is guaranteed that the union of all of your connections and your competitor's connections form a connected network.</p>

## Output

<p>Print a single integer, the maximum possible profit you can achieve if you set the prices on your connections appropriately. If the profit is unbounded, print $-1$.</p>





```input1
4 3 6
1 2
3 4
1 3
2 3 3
3 1 4
1 2 4
4 2 8
4 3 8
4 1 10

```




```input2
3 2 1
1 2
2 3
1 2 30

```




```input3
4 3 3
1 2
1 3
1 4
4 1 1000000000
4 2 1000000000
4 3 1000000000

```




```output1
14

```




```output2
-1

```




```output3
3000000000

```



## Note

<p>In the first sample, it's optimal to give connection $1-3$ cost $3$, connection $1-2$ cost $3$, and connection $3-4$ cost $8$. In this case, the cheapest connected network has cost $14$, and the customer will choose one that chooses all of your connections.</p><p>In the second sample, as long as your first connection costs $30$ or less, the customer chooses both your connections no matter what is the cost of the second connection, so you can get unbounded profit in this case.</p>
