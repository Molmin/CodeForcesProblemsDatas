## Description

<div><p>The new pedestrian zone in Moscow city center consists of $n$ squares connected with each other by $n - 1$ footpaths. We define a <span class="tex-font-style-it">simple path</span> as a sequence of squares such that no square appears in this sequence twice and any two adjacent squares in this sequence are directly connected with a footpath. The size of a simple path is the number of squares in it. The footpaths are designed in a such a way that there is exactly one simple path between any pair of different squares.</p><p>During preparations for Moscow City Day the city council decided to renew ground tiles on all $n$ squares. There are $k$ tile types of different colors, numbered from $1$ to $k$. For each square exactly one tile type must be selected and then used to cover this square surface. To make walking through the city center more fascinating, it was decided to select tiles types for each square in such a way that any possible simple path of size exactly $k$ contains squares with all $k$ possible tile colors.</p><p>You need to find out whether it is possible to place the tiles this way or not.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $k$ ($2 \le k \le n \le 200\,000$)&nbsp;— the number of squares in the new pedestrian zone, the number of different tile colors.</p><p>Each of the following $n - 1$ lines contains two integers $v_i$ and $u_i$ ($1 \le v_i, u_i \le n$)&nbsp;— numbers of the squares connected by the corresponding road.</p><p>It's guaranteed, that it's possible to go from any square to any other square, moreover there is exactly one such simple path.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" if it is possible to assign tile colors this way and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>In case your answer is "<span class="tex-font-style-tt">Yes</span>", print $n$ integers from $1$ to $k$ each, the color of the tile for every square.</p></div>

## Input

<p>The first line contains two integers $n$, $k$ ($2 \le k \le n \le 200\,000$)&nbsp;— the number of squares in the new pedestrian zone, the number of different tile colors.</p><p>Each of the following $n - 1$ lines contains two integers $v_i$ and $u_i$ ($1 \le v_i, u_i \le n$)&nbsp;— numbers of the squares connected by the corresponding road.</p><p>It's guaranteed, that it's possible to go from any square to any other square, moreover there is exactly one such simple path.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" if it is possible to assign tile colors this way and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>In case your answer is "<span class="tex-font-style-tt">Yes</span>", print $n$ integers from $1$ to $k$ each, the color of the tile for every square.</p>





```input1
7 4
1 3
2 3
3 4
4 5
5 6
5 7
```




```input2
7 3
1 3
2 3
3 4
4 5
5 6
5 7
```




```output1
Yes
1 1 2 3 4 1 1
```




```output2
No
```



## Note

<p>The following pictures illustrate the pedestrian zone in first and second examples. The second picture also shows one possible distribution of colors among the squares for $k = 4$.</p><center> <img class="tex-graphics" src="file://ZCxZA3BS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
