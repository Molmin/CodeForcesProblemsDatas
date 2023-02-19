## Description

<div><p>SWERC organizers want to hold a gastronomic event.</p><p>The location of the event is a building with $n$ rooms connected by $n-1$ corridors (each corridor connects two rooms) so that it is possible to go from any room to any other room.</p><p>In each room you have to set up the tasting of a typical Italian dish. You can choose from $n$ typical Italian dishes rated from $1$ to $n$ depending on how good they are ($n$ is the best possible rating). The $n$ dishes have distinct ratings.</p><p>You want to assign the $n$ dishes to the $n$ rooms so that the number of pleasing tours is maximal. A <span class="tex-font-style-it">pleasing tour</span> is a nonempty sequence of rooms so that:</p><ul> <li> Each room in the sequence is connected to the next one in the sequence by a corridor. </li><li> The ratings of the dishes in the rooms (in the order given by the sequence) are increasing. </li></ul> If you assign the $n$ dishes optimally, what is the maximum number of pleasing tours?</div><div class="input-specification"><p>The first line contains an integer $n$ ($2\le n\le 1\,000\,000$) — the number of rooms.</p><p>The second line contains $n-1$ integers $p_2, p_3, \cdots , p_n$ ($1 \leq p_i &lt; i$). Each $p_i$ indicates that there is a corridor between room $i$ and room $p_i$. It is guaranteed that the building has the property that it is possible to go from any room to any other room.</p></div><div class="output-specification"><p>Print the maximum number of pleasing tours.</p></div>

## Input

<p>The first line contains an integer $n$ ($2\le n\le 1\,000\,000$) — the number of rooms.</p><p>The second line contains $n-1$ integers $p_2, p_3, \cdots , p_n$ ($1 \leq p_i &lt; i$). Each $p_i$ indicates that there is a corridor between room $i$ and room $p_i$. It is guaranteed that the building has the property that it is possible to go from any room to any other room.</p>

## Output

<p>Print the maximum number of pleasing tours.</p>





```input1
5
1 2 2 2
```




```input2
10
1 2 3 4 3 2 7 8 7
```




```output1
13
```




```output2
47
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, it is optimal to place the dish with rating $1$ in room $1$, the dish with rating $2$ in room $3$, the dish with rating $3$ in room $2$, the dish with rating $4$ in room $5$ and the dish with rating $5$ in room $4$. </p><p>All the $13$ possible pleasing tours are: $(1)$, $(2)$, $(3)$, $(4)$, $(5)$, $(1,2)$, $(3,2)$, $(2,4)$, $(2,5)$, $(1,2,4)$, $(1,2,5)$, $(3,2,4)$, $(3,2,5)$.</p><p>There are also other ways to assign the dishes to the rooms so that there are $13$ pleasing tours.</p>
