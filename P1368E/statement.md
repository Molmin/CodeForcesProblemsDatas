## Description

<div><p>Arthur owns a ski resort on a mountain. There are $n$ landing spots on the mountain numbered from $1$ to $n$ from the top to the foot of the mountain. The spots are connected with one-directional ski tracks. All tracks go towards the foot of the mountain, so there are <span class="tex-font-style-bf">no directed cycles</span> formed by the tracks. There are <span class="tex-font-style-bf">at most two tracks leaving each spot</span>, but many tracks may enter the same spot.</p><p>A skier can start skiing from one spot and stop in another spot if there is a sequence of tracks that lead from the starting spot and end in the ending spot. Unfortunately, recently there were many accidents, because the structure of the resort allows a skier to go through dangerous paths, by reaching high speed and endangering himself and the other customers. Here, a path is called dangerous, if it consists of at least two tracks.</p><p>Arthur wants to secure his customers by closing some of the spots in a way that there are no dangerous paths in the resort. When a spot is closed, all tracks entering and leaving that spot become unusable. </p><p>Formally, after closing some of the spots, <span class="tex-font-style-bf">there should not be a path that consists of two or more tracks</span>.</p><p>Arthur doesn't want to close too many spots. He will be happy to find any way to close <span class="tex-font-style-bf">at most $\frac{4}{7}n$ spots</span> so that the remaining part is safe. Help him find any suitable way to do so.</p></div><div class="input-specification"><p>The first line contains a single positive integer $T$&nbsp;— the number of test cases. $T$ test case description follows.</p><p>The first line of each description contains two integers $n$ and $m$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of landing spots and tracks respectively.</p><p>The following $m$ lines describe the tracks. Each of these lines contains two integers $x$ and $y$ ($1 \leq x &lt; y \leq n$)&nbsp;— indices of the starting and finishing spots for the respective track. It is guaranteed that at most two tracks start at each spot. There may be tracks in which starting and finishing spots both coincide.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer $k$ ($0 \leq k \leq \frac{4}{7}n$)&nbsp;— the number of spots to be closed. In the next line, print $k$ distinct integers&nbsp;— indices of all spots to be closed, in any order.</p><p>If there are several answers, you may output any of them. Note that you <span class="tex-font-style-bf">don't have to minimize $k$</span>. It can be shown that a suitable answer always exists.</p></div>

## Input

<p>The first line contains a single positive integer $T$&nbsp;— the number of test cases. $T$ test case description follows.</p><p>The first line of each description contains two integers $n$ and $m$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of landing spots and tracks respectively.</p><p>The following $m$ lines describe the tracks. Each of these lines contains two integers $x$ and $y$ ($1 \leq x &lt; y \leq n$)&nbsp;— indices of the starting and finishing spots for the respective track. It is guaranteed that at most two tracks start at each spot. There may be tracks in which starting and finishing spots both coincide.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer $k$ ($0 \leq k \leq \frac{4}{7}n$)&nbsp;— the number of spots to be closed. In the next line, print $k$ distinct integers&nbsp;— indices of all spots to be closed, in any order.</p><p>If there are several answers, you may output any of them. Note that you <span class="tex-font-style-bf">don't have to minimize $k$</span>. It can be shown that a suitable answer always exists.</p>





```input1
2
4 6
1 2
1 3
2 3
2 4
3 4
3 4
7 6
1 2
1 3
2 4
2 5
3 6
3 7
```




```output1
2
3 4 
4
4 5 6 7
```



## Note

<p>In the first sample case, closing any two spots is suitable.</p><p>In the second sample case, closing only the spot $1$ is also suitable.</p>
