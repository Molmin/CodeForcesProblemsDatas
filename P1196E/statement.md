## Description

<div><p>You are given two integers $b$ and $w$. You have a chessboard of size $10^9 \times 10^9$ with the top left cell at $(1; 1)$, the cell $(1; 1)$ is painted <span class="tex-font-style-bf">white</span>.</p><p>Your task is to find a connected component on this chessboard that contains exactly $b$ black cells and exactly $w$ white cells. Two cells are called connected if they share a side (i.e. for the cell $(x, y)$ there are at most four connected cells: $(x - 1, y), (x + 1, y), (x, y - 1), (x, y + 1)$). A set of cells is called a connected component if for every pair of cells $C_1$ and $C_2$ from this set, there exists a sequence of cells $c_1$, $c_2$, ..., $c_k$ such that $c_1 = C_1$, $c_k = C_2$, all $c_i$ from $1$ to $k$ are belong to this set of cells and for every $i \in [1, k - 1]$, cells $c_i$ and $c_{i + 1}$ are connected.</p><p>Obviously, it can be impossible to find such component. In this case print "<span class="tex-font-style-tt">NO</span>". Otherwise, print "<span class="tex-font-style-tt">YES</span>" and <span class="tex-font-style-bf">any</span> suitable connected component.</p><p>You have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries. Then $q$ queries follow.</p><p>The only line of the query contains two integers $b$ and $w$ ($1 \le b, w \le 10^5$)&nbsp;— the number of black cells required and the number of white cells required.</p><p>It is guaranteed that the sum of numbers of cells does not exceed $2 \cdot 10^5$ ($\sum w + \sum b \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each query, print the answer to it.</p><p>If it is impossible to find the required component, print "<span class="tex-font-style-tt">NO</span>" on the first line.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" on the first line. In the next $b + w$ lines print coordinates of cells of your component in any order. There should be exactly $b$ black cells and $w$ white cells in your answer. The printed component should be connected.</p><p>If there are several answers, you can print <span class="tex-font-style-bf">any</span>. All coordinates in the answer should be in the range $[1; 10^9]$.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries. Then $q$ queries follow.</p><p>The only line of the query contains two integers $b$ and $w$ ($1 \le b, w \le 10^5$)&nbsp;— the number of black cells required and the number of white cells required.</p><p>It is guaranteed that the sum of numbers of cells does not exceed $2 \cdot 10^5$ ($\sum w + \sum b \le 2 \cdot 10^5$).</p>

## Output

<p>For each query, print the answer to it.</p><p>If it is impossible to find the required component, print "<span class="tex-font-style-tt">NO</span>" on the first line.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" on the first line. In the next $b + w$ lines print coordinates of cells of your component in any order. There should be exactly $b$ black cells and $w$ white cells in your answer. The printed component should be connected.</p><p>If there are several answers, you can print <span class="tex-font-style-bf">any</span>. All coordinates in the answer should be in the range $[1; 10^9]$.</p>





```input1
3
1 1
1 4
2 5
```




```output1
YES
2 2
1 2
YES
2 3
1 3
3 3
2 2
2 4
YES
2 3
2 4
2 5
1 3
1 5
3 3
3 5
```


