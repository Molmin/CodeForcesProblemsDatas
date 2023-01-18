## Description

<div><p>You are given a tree consisting of $n$ vertices. A tree is an undirected connected acyclic graph.</p><center> <img class="tex-graphics" src="file://YUrenzxd.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Example of a tree.</span> </center><p>You have to paint each vertex into one of three colors. For each vertex, you know the cost of painting it in every color.</p><p>You have to paint the vertices so that any path consisting of exactly three distinct vertices does not contain any vertices with equal colors. In other words, let's consider all triples $(x, y, z)$ such that $x \neq y, y \neq z, x \neq z$, $x$ is connected by an edge with $y$, and $y$ is connected by an edge with $z$. The colours of $x$, $y$ and $z$ should be pairwise distinct. Let's call a painting which meets this condition <span class="tex-font-style-it">good</span>.</p><p>You have to calculate the minimum cost of a <span class="tex-font-style-it">good</span> painting and find one of the optimal paintings. If there is no <span class="tex-font-style-it">good</span> painting, report about it.</p></div><div class="input-specification"><p>The first line contains one integer $n$ $(3 \le n \le 100\,000)$ — the number of vertices.</p><p>The second line contains a sequence of integers $c_{1, 1}, c_{1, 2}, \dots, c_{1, n}$ $(1 \le c_{1, i} \le 10^{9})$, where $c_{1, i}$ is the cost of painting the $i$-th vertex into the first color.</p><p>The third line contains a sequence of integers $c_{2, 1}, c_{2, 2}, \dots, c_{2, n}$ $(1 \le c_{2, i} \le 10^{9})$, where $c_{2, i}$ is the cost of painting the $i$-th vertex into the second color.</p><p>The fourth line contains a sequence of integers $c_{3, 1}, c_{3, 2}, \dots, c_{3, n}$ $(1 \le c_{3, i} \le 10^{9})$, where $c_{3, i}$ is the cost of painting the $i$-th vertex into the third color.</p><p>Then $(n - 1)$ lines follow, each containing two integers $u_j$ and $v_j$ $(1 \le u_j, v_j \le n, u_j \neq v_j)$ — the numbers of vertices connected by the $j$-th undirected edge. It is guaranteed that these edges denote a tree.</p></div><div class="output-specification"><p>If there is no <span class="tex-font-style-it">good</span> painting, print $-1$.</p><p>Otherwise, print the minimum cost of a <span class="tex-font-style-it">good</span> painting in the first line. In the second line print $n$ integers $b_1, b_2, \dots, b_n$ $(1 \le b_i \le 3)$, where the $i$-th integer should denote the color of the $i$-th vertex. If there are multiple good paintings with minimum cost, print any of them.</p></div>

## Input

<p>The first line contains one integer $n$ $(3 \le n \le 100\,000)$ — the number of vertices.</p><p>The second line contains a sequence of integers $c_{1, 1}, c_{1, 2}, \dots, c_{1, n}$ $(1 \le c_{1, i} \le 10^{9})$, where $c_{1, i}$ is the cost of painting the $i$-th vertex into the first color.</p><p>The third line contains a sequence of integers $c_{2, 1}, c_{2, 2}, \dots, c_{2, n}$ $(1 \le c_{2, i} \le 10^{9})$, where $c_{2, i}$ is the cost of painting the $i$-th vertex into the second color.</p><p>The fourth line contains a sequence of integers $c_{3, 1}, c_{3, 2}, \dots, c_{3, n}$ $(1 \le c_{3, i} \le 10^{9})$, where $c_{3, i}$ is the cost of painting the $i$-th vertex into the third color.</p><p>Then $(n - 1)$ lines follow, each containing two integers $u_j$ and $v_j$ $(1 \le u_j, v_j \le n, u_j \neq v_j)$ — the numbers of vertices connected by the $j$-th undirected edge. It is guaranteed that these edges denote a tree.</p>

## Output

<p>If there is no <span class="tex-font-style-it">good</span> painting, print $-1$.</p><p>Otherwise, print the minimum cost of a <span class="tex-font-style-it">good</span> painting in the first line. In the second line print $n$ integers $b_1, b_2, \dots, b_n$ $(1 \le b_i \le 3)$, where the $i$-th integer should denote the color of the $i$-th vertex. If there are multiple good paintings with minimum cost, print any of them.</p>





```input1
3
3 2 3
4 3 2
3 1 3
1 2
2 3
```




```input2
5
3 4 2 1 2
4 2 1 5 4
5 3 2 1 1
1 2
3 2
4 3
5 3
```




```input3
5
3 4 2 1 2
4 2 1 5 4
5 3 2 1 1
1 2
3 2
4 3
5 4
```




```output1
6
1 3 2
```




```output2
-1
```




```output3
9
1 3 2 1 3
```



## Note

<p>All vertices should be painted in different colors in the first example. The optimal way to do it is to paint the first vertex into color $1$, the second vertex — into color $3$, and the third vertex — into color $2$. The cost of this painting is $3 + 2 + 1 = 6$.</p>
