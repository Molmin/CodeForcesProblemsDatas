## Description

<div><p>The city of Fishtopia can be imagined as a grid of $4$ rows and an <span class="tex-font-style-bf">odd</span> number of columns. It has two main villages; the first is located at the top-left cell $(1,1)$, people who stay there love fishing at the Tuna pond at the bottom-right cell $(4, n)$. The second village is located at $(4, 1)$ and its people love the Salmon pond at $(1, n)$.</p><p>The mayor of Fishtopia wants to place $k$ hotels in the city, each one occupying one cell. To allow people to enter the city from anywhere, hotels should not be placed on the border cells.</p><p>A person can move from one cell to another if those cells are not occupied by hotels and share a side.</p><p>Can you help the mayor place the hotels in a way such that there are equal number of shortest paths from each village to its preferred pond?</p></div><div class="input-specification"><p>The first line of input contain two integers, $n$ and $k$ ($3 \leq n \leq 99$, $0 \leq k \leq 2\times(n-2)$), $n$ is <span class="tex-font-style-bf">odd</span>, the width of the city, and the number of hotels to be placed, respectively.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>", if it is possible to place all the hotels in a way that satisfies the problem statement, otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>If it is possible, print an extra $4$ lines that describe the city, each line should have $n$ characters, each of which is "<span class="tex-font-style-tt">#</span>" if that cell has a hotel on it, or "<span class="tex-font-style-tt">.</span>" if not.</p></div>

## Input

<p>The first line of input contain two integers, $n$ and $k$ ($3 \leq n \leq 99$, $0 \leq k \leq 2\times(n-2)$), $n$ is <span class="tex-font-style-bf">odd</span>, the width of the city, and the number of hotels to be placed, respectively.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>", if it is possible to place all the hotels in a way that satisfies the problem statement, otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>If it is possible, print an extra $4$ lines that describe the city, each line should have $n$ characters, each of which is "<span class="tex-font-style-tt">#</span>" if that cell has a hotel on it, or "<span class="tex-font-style-tt">.</span>" if not.</p>





```input1
7 2

```




```input2
5 3

```




```output1
YES
.......
.#.....
.#.....
.......

```




```output2
YES
.....
.###.
.....
.....

```


