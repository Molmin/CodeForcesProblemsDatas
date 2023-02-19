## Description

<div><p>In this problem, we will be working with rooted binary trees. A tree is called a rooted binary tree if it has a fixed root and every vertex has at most two children.</p><p>Let's assign a color&nbsp;— white or blue&nbsp;— to each vertex of the tree, and call this assignment a <span class="tex-font-style-it">coloring</span> of the tree. Let's call a coloring <span class="tex-font-style-it">diverse</span> if every vertex has a neighbor (a parent or a child) colored into an opposite color compared to this vertex. It can be shown that any tree with at least two vertices allows a diverse coloring.</p><p>Let's define the <span class="tex-font-style-it">disbalance</span> of a coloring as the absolute value of the difference between the number of white vertices and the number of blue vertices.</p><p>Now to the problem. Initially, the tree consists of a single vertex with the number $1$ which is its root. Then, for each $i$ from $2$ to $n$, a new vertex $i$ appears in the tree, and it becomes a child of vertex $p_i$. It is guaranteed that after each step the tree will keep being a binary tree rooted at vertex $1$, that is, each vertex will have at most two children.</p><p>After every new vertex is added, print the smallest value of disbalance over all possible diverse colorings of the current tree. Moreover, after adding the last vertex with the number $n$, also print a diverse coloring with the smallest possible disbalance as well.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$&nbsp;($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the final tree.</p><p>The second line contains $n-1$ integers $p_2, p_3, \ldots, p_n$&nbsp;($1 \le p_i \le i - 1$)&nbsp;— the numbers of parents of vertices $2, 3, \ldots, n$. No integer appears more than twice among $p_2, p_3, \ldots, p_n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print $n-1$ integers&nbsp;— the smallest value of disbalance over all possible diverse colorings of the tree after adding vertices $2, 3, \ldots, n$.</p><p>Then print a string of $n$ characters '<span class="tex-font-style-tt">w</span>' and '<span class="tex-font-style-tt">b</span>', describing a diverse coloring with the smallest possible disbalance for the whole tree after adding vertex $n$: the $i$-th character must be equal to '<span class="tex-font-style-tt">w</span>' if vertex $i$ is colored white, and '<span class="tex-font-style-tt">b</span>' if it's colored blue. The absolute value of the difference between the numbers of '<span class="tex-font-style-tt">w</span>' and '<span class="tex-font-style-tt">b</span>' characters must be equal to the last printed integer. Each vertex must have a parent or a child colored into the color opposite to the vertex's color.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$&nbsp;($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the final tree.</p><p>The second line contains $n-1$ integers $p_2, p_3, \ldots, p_n$&nbsp;($1 \le p_i \le i - 1$)&nbsp;— the numbers of parents of vertices $2, 3, \ldots, n$. No integer appears more than twice among $p_2, p_3, \ldots, p_n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print $n-1$ integers&nbsp;— the smallest value of disbalance over all possible diverse colorings of the tree after adding vertices $2, 3, \ldots, n$.</p><p>Then print a string of $n$ characters '<span class="tex-font-style-tt">w</span>' and '<span class="tex-font-style-tt">b</span>', describing a diverse coloring with the smallest possible disbalance for the whole tree after adding vertex $n$: the $i$-th character must be equal to '<span class="tex-font-style-tt">w</span>' if vertex $i$ is colored white, and '<span class="tex-font-style-tt">b</span>' if it's colored blue. The absolute value of the difference between the numbers of '<span class="tex-font-style-tt">w</span>' and '<span class="tex-font-style-tt">b</span>' characters must be equal to the last printed integer. Each vertex must have a parent or a child colored into the color opposite to the vertex's color.</p>





```input1|2,3
2
7
1 2 2 1 5 5
8
1 2 3 4 5 6 7
```




```output1
0
1
2
1
0
1
wbwwwbb
0
1
0
1
0
1
0
wbwbwbwb
```



## Note

<p>In the first test case, examples of diverse colorings with the smallest possible disbalances for all intermediate trees are illustrated below:</p><center> <img class="tex-graphics" src="file://4uuveQmy.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
