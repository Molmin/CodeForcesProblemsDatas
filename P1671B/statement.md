## Description

<div><p>You are given $n$ points with integer coordinates on a coordinate axis $OX$. The coordinate of the $i$-th point is $x_i$. All points' coordinates are distinct and given in strictly increasing order.</p><p>For each point $i$, you can do the following operation <span class="tex-font-style-bf">no more than once</span>: take this point and move it by $1$ to the left or to the right (i..e., you can change its coordinate $x_i$ to $x_i - 1$ or to $x_i + 1$). In other words, for each point, you choose (separately) its new coordinate. For the $i$-th point, it can be either $x_i - 1$, $x_i$ or $x_i + 1$.</p><p>Your task is to determine if you can move some points as described above in such a way that the new set of points forms a <span class="tex-font-style-bf">consecutive segment</span> of integers, i. e. for some integer $l$ the coordinates of points should be equal to $l, l + 1, \ldots, l + n - 1$.</p><p>Note that the resulting points should have <span class="tex-font-style-bf">distinct</span> coordinates.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of points in the set $x$.</p><p>The second line of the test case contains $n$ integers $x_1 &lt; x_2 &lt; \ldots &lt; x_n$ ($1 \le x_i \le 10^6$), where $x_i$ is the coordinate of the $i$-th point.</p><p>It is guaranteed that the points are given in strictly increasing order (this also means that all coordinates are distinct). It is also guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer — if the set of points from the test case can be moved to form a consecutive segment of integers, print <span class="tex-font-style-tt">YES</span>, otherwise print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of points in the set $x$.</p><p>The second line of the test case contains $n$ integers $x_1 &lt; x_2 &lt; \ldots &lt; x_n$ ($1 \le x_i \le 10^6$), where $x_i$ is the coordinate of the $i$-th point.</p><p>It is guaranteed that the points are given in strictly increasing order (this also means that all coordinates are distinct). It is also guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer — if the set of points from the test case can be moved to form a consecutive segment of integers, print <span class="tex-font-style-tt">YES</span>, otherwise print <span class="tex-font-style-tt">NO</span>.</p>





```input1
5
2
1 4
3
1 2 3
4
1 2 3 7
1
1000000
3
2 5 6
```




```output1
YES
YES
NO
YES
YES
```


