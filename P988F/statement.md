## Description

<div><p>Polycarp lives on a coordinate line at the point $x = 0$. He goes to his friend that lives at the point $x = a$. Polycarp can move only from left to right, he can pass one unit of length each second.</p><p>Now it's raining, so some segments of his way are in the rain. Formally, it's raining on $n$ non-intersecting segments, the $i$-th segment which is in the rain is represented as $[l_i, r_i]$ ($0 \le l_i &lt; r_i \le a$).</p><p>There are $m$ umbrellas lying on the line, the $i$-th umbrella is located at point $x_i$ ($0 \le x_i \le a$) and has weight $p_i$. When Polycarp begins his journey, he doesn't have any umbrellas.</p><p>During his journey from $x = 0$ to $x = a$ Polycarp can pick up and throw away umbrellas. Polycarp picks up and throws down any umbrella instantly. He can carry any number of umbrellas at any moment of time. Because Polycarp doesn't want to get wet, he must carry at least one umbrella while he moves from $x$ to $x + 1$ if a segment $[x, x + 1]$ is in the rain (i.e. if there exists some $i$ such that $l_i \le x$ and $x + 1 \le r_i$).</p><p>The condition above is the only requirement. For example, it is possible to go without any umbrellas to a point where some rain segment starts, pick up an umbrella at this point and move along with an umbrella. Polycarp can swap umbrellas while he is in the rain.</p><p>Each unit of length passed increases Polycarp's fatigue by the sum of the weights of umbrellas he carries while moving.</p><p>Can Polycarp make his way from point $x = 0$ to point $x = a$? If yes, find the minimum total fatigue after reaching $x = a$, if Polycarp picks up and throws away umbrellas optimally.</p></div><div class="input-specification"><p>The first line contains three integers $a$, $n$ and $m$ ($1 \le a, m \le 2000, 1 \le n \le \lceil\frac{a}{2}\rceil$) — the point at which Polycarp's friend lives, the number of the segments in the rain and the number of umbrellas.</p><p>Each of the next $n$ lines contains two integers $l_i$ and $r_i$ ($0 \le l_i &lt; r_i \le a$) — the borders of the $i$-th segment under rain. <span class="tex-font-style-bf">It is guaranteed that there is no pair of intersecting segments</span>. In other words, for each pair of segments $i$ and $j$ either $r_i &lt; l_j$ or $r_j &lt; l_i$.</p><p>Each of the next $m$ lines contains two integers $x_i$ and $p_i$ ($0 \le x_i \le a$, $1 \le p_i \le 10^5$) — the location and the weight of the $i$-th umbrella.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">-1</span>" (without quotes) if Polycarp can't make his way from point $x = 0$ to point $x = a$. Otherwise print one integer — the minimum total fatigue after reaching $x = a$, if Polycarp picks up and throws away umbrellas optimally.</p></div>

## Input

<p>The first line contains three integers $a$, $n$ and $m$ ($1 \le a, m \le 2000, 1 \le n \le \lceil\frac{a}{2}\rceil$) — the point at which Polycarp's friend lives, the number of the segments in the rain and the number of umbrellas.</p><p>Each of the next $n$ lines contains two integers $l_i$ and $r_i$ ($0 \le l_i &lt; r_i \le a$) — the borders of the $i$-th segment under rain. <span class="tex-font-style-bf">It is guaranteed that there is no pair of intersecting segments</span>. In other words, for each pair of segments $i$ and $j$ either $r_i &lt; l_j$ or $r_j &lt; l_i$.</p><p>Each of the next $m$ lines contains two integers $x_i$ and $p_i$ ($0 \le x_i \le a$, $1 \le p_i \le 10^5$) — the location and the weight of the $i$-th umbrella.</p>

## Output

<p>Print "<span class="tex-font-style-tt">-1</span>" (without quotes) if Polycarp can't make his way from point $x = 0$ to point $x = a$. Otherwise print one integer — the minimum total fatigue after reaching $x = a$, if Polycarp picks up and throws away umbrellas optimally.</p>





```input1
10 2 4
3 7
8 10
0 10
3 4
8 1
1 2

```




```input2
10 1 1
0 9
0 5

```




```input3
10 1 1
0 9
1 5

```




```output1
14

```




```output2
45

```




```output3
-1

```



## Note

<p>In the first example the only possible strategy is to take the fourth umbrella at the point $x = 1$, keep it till the point $x = 7$ (the total fatigue at $x = 7$ will be equal to $12$), throw it away, move on from $x = 7$ to $x = 8$ without an umbrella, take the third umbrella at $x = 8$ and keep it till the end (the total fatigue at $x = 10$ will be equal to $14$). </p><p>In the second example the only possible strategy is to take the first umbrella, move with it till the point $x = 9$, throw it away and proceed without an umbrella till the end.</p>
