## Description

<div><p>There is a strip with an infinite number of cells. Cells are numbered starting with $0$. Initially the cell $i$ contains a ball with the number $i$.</p><p>There are $n$ pockets located at cells $a_1, \ldots, a_n$. Each cell contains at most one pocket.</p><p><span class="tex-font-style-it">Filtering</span> is the following sequence of operations:</p><ul><li> All pockets at cells $a_1, \ldots, a_n$ open simultaneously, which makes balls currently located at those cells disappear. After the balls disappear, the pockets close again.</li><li> For each cell $i$ from $0$ to $\infty$, if the cell $i$ contains a ball, we move that ball to the free cell $j$ with the lowest number. If there is no free cell $j &lt; i$, the ball stays at the cell $i$.</li></ul><p>Note that after each filtering operation each cell will still contain exactly one ball.</p><p>For example, let the cells $1$, $3$ and $4$ contain pockets. The initial configuration of balls is shown below (underscores display the cells with pockets):</p><center> 0 <span class="tex-font-style-underline">1</span> 2 <span class="tex-font-style-underline">3</span> <span class="tex-font-style-underline">4</span> 5 6 7 8 9 ... </center><p>After opening and closing the pockets, balls 1, 3 and 4 disappear:</p><center> 0 <span class="tex-font-style-underline">&nbsp;</span> 2 <span class="tex-font-style-underline">&nbsp;</span> <span class="tex-font-style-underline">&nbsp;</span> 5 6 7 8 9 ... </center><p>After moving all the balls to the left, the configuration looks like this:</p><center> 0 <span class="tex-font-style-underline">2</span> 5 <span class="tex-font-style-underline">6</span> <span class="tex-font-style-underline">7</span> 8 9 10 11 12 ... </center><p>Another filtering repetition results in the following:</p><center> 0 <span class="tex-font-style-underline">5</span> 8 <span class="tex-font-style-underline">9</span> <span class="tex-font-style-underline">10</span> 11 12 13 14 15 ... </center><p>You have to answer $m$ questions. The $i$-th of these questions is "what is the number of the ball located at the cell $x_i$ after $k_i$ repetitions of the filtering operation?"</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$&nbsp;— the number of pockets and questions respectively ($1 \leq n, m \leq 10^5$).</p><p>The following line contains $n$ integers $a_1, \ldots, a_n$&nbsp;— the numbers of cells containing pockets ($0 \leq a_1 &lt; \ldots &lt; a_n \leq 10^9$).</p><p>The following $m$ lines describe questions. The $i$-th of these lines contains two integers $x_i$ and $k_i$ ($0 \leq x_i, k_i \leq 10^9$).</p></div><div class="output-specification"><p>Print $m$ numbers&nbsp;— answers to the questions, in the same order as given in the input.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$&nbsp;— the number of pockets and questions respectively ($1 \leq n, m \leq 10^5$).</p><p>The following line contains $n$ integers $a_1, \ldots, a_n$&nbsp;— the numbers of cells containing pockets ($0 \leq a_1 &lt; \ldots &lt; a_n \leq 10^9$).</p><p>The following $m$ lines describe questions. The $i$-th of these lines contains two integers $x_i$ and $k_i$ ($0 \leq x_i, k_i \leq 10^9$).</p>

## Output

<p>Print $m$ numbers&nbsp;— answers to the questions, in the same order as given in the input.</p>





```input1
3 15
1 3 4
0 0
1 0
2 0
3 0
4 0
0 1
1 1
2 1
3 1
4 1
0 2
1 2
2 2
3 2
4 2

```




```output1
0
1
2
3
4
0
2
5
6
7
0
5
8
9
10

```


