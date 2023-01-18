## Description

<div><p>Vova has recently learned what a <span class="tex-font-style-it">circulaton</span> in a graph is. Recall the definition: let $G = (V, E)$ be a directed graph. A circulation $f$ is such a collection of non-negative real numbers $f_e$ ($e \in E$), that for each vertex $v \in V$ the following <span class="tex-font-style-it">conservation</span> condition holds:</p><p>$$\sum\limits_{e \in \delta^{-}(v)} f_e = \sum\limits_{e \in \delta^{+}(v)} f_e$$</p><p>where $\delta^{+}(v)$ is the set of edges that end in the vertex $v$, and $\delta^{-}(v)$ is the set of edges that start in the vertex $v$. In other words, for each vertex the total incoming flow should be equal to the total outcoming flow.</p><p>Let a $lr$-circulation be such a circulation $f$ that for each edge the condition $l_e \leq f_e \leq r_e$ holds, where $l_e$ and $r_e$ for each edge $e \in E$ are two non-negative real numbers denoting the lower and upper bounds on the value of the circulation on this edge $e$.</p><p>Vova can't stop thinking about applications of a new topic. Right now he thinks about the following <span class="tex-font-style-it">natural</span> question: let the graph be fixed, and each value $l_e$ and $r_e$ be a linear function of a real variable $t$:</p><p>$$l_e(t) = a_e t + b_e$$ $$r_e(t) = c_e t + d_e$$</p><p>Note that $t$ is the <span class="tex-font-style-bf">same</span> for all edges.</p><p>Let $t$ be chosen at random from uniform distribution on a segment $[0, 1]$. What is the probability of existence of $lr$-circulation in the graph?</p></div><div class="input-specification"><p>The first line contains two integers $n$, $m$ ($1 \leq n \leq 1000$, $1 \leq m \leq 2000$).</p><p>Each of the next $m$ lines describes edges of the graph in the format $u_e$, $v_e$, $a_e$, $b_e$, $c_e$, $d_e$ ($1 \leq u_e, v_e \leq n$, $-10^4 \leq a_e, c_e \leq 10^4$, $0 \leq b_e, d_e \leq 10^4$), where $u_e$ and $v_e$ are the startpoint and the endpoint of the edge $e$, and the remaining 4 integers describe the linear functions for the upper and lower bound of circulation.</p><p>It is guaranteed that for any $t \in [0, 1]$ and for any edge $e \in E$ the following condition holds $0 \leq l_e(t) \leq r_e(t) \leq 10^4$.</p></div><div class="output-specification"><p>Print a single real integer — the probability of existence of $lr$-circulation in the graph, given that $t$ is chosen uniformly at random from the segment $[0, 1]$. Your answer is considered correct if its absolute difference from jury's answer is not greater than $10^{-6}$.</p></div>

## Input

<p>The first line contains two integers $n$, $m$ ($1 \leq n \leq 1000$, $1 \leq m \leq 2000$).</p><p>Each of the next $m$ lines describes edges of the graph in the format $u_e$, $v_e$, $a_e$, $b_e$, $c_e$, $d_e$ ($1 \leq u_e, v_e \leq n$, $-10^4 \leq a_e, c_e \leq 10^4$, $0 \leq b_e, d_e \leq 10^4$), where $u_e$ and $v_e$ are the startpoint and the endpoint of the edge $e$, and the remaining 4 integers describe the linear functions for the upper and lower bound of circulation.</p><p>It is guaranteed that for any $t \in [0, 1]$ and for any edge $e \in E$ the following condition holds $0 \leq l_e(t) \leq r_e(t) \leq 10^4$.</p>

## Output

<p>Print a single real integer — the probability of existence of $lr$-circulation in the graph, given that $t$ is chosen uniformly at random from the segment $[0, 1]$. Your answer is considered correct if its absolute difference from jury's answer is not greater than $10^{-6}$.</p>





```input1
3 3
1 2 0 3 -4 7
2 3 -2 5 1 6
3 1 0 4 0 4

```




```output1
0.25
```



## Note

<p>In the first example the conservation condition allows only circulations with equal values $f_e$ for all three edges. The value of circulation on the last edge should be $4$ whatever $t$ is chosen, so the probability is</p><p>$$P(4 \in [3, -4t + 7]~~\&amp;~~4 \in [-2t + 5, t + 6]) = 0.25$$</p>
