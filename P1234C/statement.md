## Description

<div><p>You are given a system of pipes. It consists of two rows, each row consists of $n$ pipes. The top left pipe has the coordinates $(1, 1)$ and the bottom right — $(2, n)$.</p><p>There are six types of pipes: two types of straight pipes and four types of curved pipes. Here are the examples of all six types:</p><center> <img class="tex-graphics" src="file://PdO2Jxjn.png" style="max-width: 100.0%;max-height: 100.0%;"> Types of pipes </center><p>You can turn each of the given pipes $90$ degrees clockwise or counterclockwise <span class="tex-font-style-bf">arbitrary (possibly, zero) number of times</span> (so the types $1$ and $2$ can become each other and types $3, 4, 5, 6$ can become each other).</p><p>You want to turn some pipes in a way that the water flow can start at $(1, 0)$ (to the left of the top left pipe), move to the pipe at $(1, 1)$, flow somehow by <span class="tex-font-style-bf">connected pipes</span> to the pipe at $(2, n)$ and flow right to $(2, n + 1)$.</p><p>Pipes are connected if they are adjacent in the system and their ends are connected. Here are examples of connected pipes:</p><center> <img class="tex-graphics" src="file://NstJP4os.png" style="max-width: 100.0%;max-height: 100.0%;"> Examples of connected pipes </center><p>Let's describe the problem using some example:</p><center> <img class="tex-graphics" src="file://bNYgECth.png" style="max-width: 100.0%;max-height: 100.0%;"> The first example input </center><p>And its solution is below: </p><center> <img class="tex-graphics" src="file://ZTBV6mJg.png" style="max-width: 100.0%;max-height: 100.0%;"> The first example answer </center><p>As you can see, the water flow is the poorly drawn blue line. To obtain the answer, we need to turn the pipe at $(1, 2)$ $90$ degrees clockwise, the pipe at $(2, 3)$ $90$ degrees, the pipe at $(1, 6)$ $90$ degrees, the pipe at $(1, 7)$ $180$ degrees and the pipe at $(2, 7)$ $180$ degrees. Then the flow of water can reach $(2, n + 1)$ from $(1, 0)$.</p><p>You have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 10^4$) — the number of queries. Then $q$ queries follow.</p><p>Each query consists of exactly three lines. The first line of the query contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of pipes in each row. The next two lines contain a description of the first and the second rows correspondingly. Each row description consists of $n$ digits from $1$ to $6$ without any whitespaces between them, each digit corresponds to the type of pipe in the corresponding cell. See the problem statement to understand which digits correspond to which types of pipes.</p><p>It is guaranteed that the sum of $n$ over all queries does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For the $i$-th query print the answer for it — "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to turn some pipes in a way that the water flow can reach $(2, n + 1)$ from $(1, 0)$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 10^4$) — the number of queries. Then $q$ queries follow.</p><p>Each query consists of exactly three lines. The first line of the query contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of pipes in each row. The next two lines contain a description of the first and the second rows correspondingly. Each row description consists of $n$ digits from $1$ to $6$ without any whitespaces between them, each digit corresponds to the type of pipe in the corresponding cell. See the problem statement to understand which digits correspond to which types of pipes.</p><p>It is guaranteed that the sum of $n$ over all queries does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For the $i$-th query print the answer for it — "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to turn some pipes in a way that the water flow can reach $(2, n + 1)$ from $(1, 0)$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
6
7
2323216
1615124
1
3
4
2
13
24
2
12
34
3
536
345
2
46
54
```




```output1
YES
YES
YES
NO
YES
NO
```



## Note

<p>The first query from the example is described in the problem statement.</p>
