## Description

<div><p>Once, during a lesson, Sasha got bored and decided to talk with his friends. Suddenly, he saw Kefa. Since we can talk endlessly about Kefa, we won't even start doing that. The conversation turned to graphs. Kefa promised Sasha to tell him about one interesting fact from graph theory if Sasha helps Kefa to count the number of <span class="tex-font-style-it">beautiful trees</span>. </p><p>In this task, a <span class="tex-font-style-it">tree</span> is a weighted connected graph, consisting of $n$ vertices and $n-1$ edges, and weights of edges are integers from $1$ to $m$. Kefa determines the beauty of a tree as follows: he finds in the tree his two favorite vertices&nbsp;— vertices with numbers $a$ and $b$, and counts the distance between them. The distance between two vertices $x$ and $y$ is the sum of weights of edges on the simple path from $x$ to $y$. If the distance between two vertices $a$ and $b$ is <span class="tex-font-style-bf">equal</span> to $m$, then the tree is <span class="tex-font-style-it">beautiful</span>.</p><p>Sasha likes graph theory, and even more, Sasha likes interesting facts, that's why he agreed to help Kefa. Luckily, Sasha is familiar with you <span class="tex-font-style-tt">the best programmer in Byteland</span>. Help Sasha to count the number of <span class="tex-font-style-it">beautiful</span> trees for Kefa. Two trees are considered to be distinct if there is an edge that occurs in one of them and doesn't occur in the other one. Edge's <span class="tex-font-style-bf">weight matters</span>.</p><p>Kefa warned Sasha, that there can be too many beautiful trees, so it will be enough to count the number modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains four integers $n$, $m$, $a$, $b$ ($2 \le n \le 10^6$, $1 \le m \le 10^6$, $1 \le a, b \le n$, $a \neq b$)&nbsp;— the number of vertices in the tree, the maximum weight of an edge and two Kefa's favorite vertices.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of <span class="tex-font-style-it">beautiful trees</span> modulo $10^9+7$.</p></div>

## Input

<p>The first line contains four integers $n$, $m$, $a$, $b$ ($2 \le n \le 10^6$, $1 \le m \le 10^6$, $1 \le a, b \le n$, $a \neq b$)&nbsp;— the number of vertices in the tree, the maximum weight of an edge and two Kefa's favorite vertices.</p>

## Output

<p>Print one integer&nbsp;— the number of <span class="tex-font-style-it">beautiful trees</span> modulo $10^9+7$.</p>





```input1
3 2 1 3
```




```input2
3 1 1 2
```




```input3
5 15 1 5
```




```output1
5
```




```output2
2
```




```output3
345444
```



## Note

<p>There are $5$ <span class="tex-font-style-it">beautiful trees</span> in the first example:</p><p><img class="tex-graphics" height="189px" src="file://uIHAxIrJ.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"></p><p>In the second example the following trees are <span class="tex-font-style-it">beautiful</span>:</p><p><img class="tex-graphics" height="265px" src="file://2ucQ8ObO.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"></p>
