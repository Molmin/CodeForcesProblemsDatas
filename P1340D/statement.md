## Description

<div><p><span class="tex-font-style-it"> Denis came to Nastya and discovered that she was not happy to see him... There is only one chance that she can become happy. Denis wants to buy all things that Nastya likes so she will certainly agree to talk to him. </span></p><p>The map of the city where they live has a lot of squares, some of which are connected by roads. There is exactly one way between each pair of squares which does not visit any vertex twice. It turns out that the graph of the city is a tree.</p><p>Denis is located at vertex $1$ at the time $0$. He wants to visit every vertex at least once and get back as soon as possible.</p><p>Denis can walk one road in $1$ time. Unfortunately, the city is so large that it will take a very long time to visit all squares. Therefore, Denis took a desperate step. He pulled out his pocket time machine, which he constructed in his basement. With its help, Denis can change the time to any non-negative time, which is less than the current time.</p><p>But the time machine has one feature. If the hero finds himself in the same place and at the same time twice, there will be an explosion of universal proportions and Nastya will stay unhappy. Therefore, Denis asks you to find him a route using a time machine that he will get around all squares and will return to the first and at the same time the maximum time in which he visited any square will be minimal.</p><p>Formally, Denis's route can be represented as a sequence of pairs: $\{v_1, t_1\}, \{v_2, t_2\}, \{v_3, t_3\}, \ldots, \{v_k, t_k\}$, where $v_i$ is number of square, and $t_i$ is time in which the boy is now.</p><p>The following conditions must be met:</p><ul> <li> The route starts on square $1$ at time $0$, i.e. $v_1 = 1, t_1 = 0$ and ends on the square $1$, i.e. $v_k = 1$. </li><li> All transitions are divided into two types: <ol> <li> Being in the square change the time: $\{ v_i, t_i \} \to \{ v_{i+1}, t_{i+1} \} : v_{i+1} = v_i, 0 \leq t_{i+1} &lt; t_i$. </li><li> Walk along one of the roads: $\{ v_i, t_i \} \to \{ v_{i+1}, t_{i+1} \}$. Herewith, $v_i$ and $v_{i+1}$ are connected by road, and $t_{i+1} = t_i + 1$ </li></ol> </li><li> All pairs $\{ v_i, t_i \}$ must be different. </li><li> All squares are among $v_1, v_2, \ldots, v_k$. </li></ul><p>You need to find a route such that the maximum time in any square will be minimal, that is, the route for which $\max{(t_1, t_2, \ldots, t_k)}$ will be the minimum possible.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ $(1 \leq n \leq 10^5)$ &nbsp;— the number of squares in the city. </p><p>The next $n - 1$ lines contain two integers $u$ and $v$ $(1 \leq v, u \leq n, u \neq v)$ - the numbers of the squares connected by the road. </p><p>It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>In the first line output the integer $k$ $(1 \leq k \leq 10^6)$ &nbsp;— the length of the path of Denis.</p><p>In the next $k$ lines output pairs $v_i, t_i$ &nbsp;— pairs that describe Denis's route (as in the statement).</p><p>All route requirements described in the statements must be met.</p><p>It is guaranteed that under given restrictions there is at least one route and an answer whose length does not exceed $10^6$. If there are several possible answers, print any.</p></div>

## Input

<p>The first line contains a single integer $n$ $(1 \leq n \leq 10^5)$ &nbsp;— the number of squares in the city. </p><p>The next $n - 1$ lines contain two integers $u$ and $v$ $(1 \leq v, u \leq n, u \neq v)$ - the numbers of the squares connected by the road. </p><p>It is guaranteed that the given graph is a tree.</p>

## Output

<p>In the first line output the integer $k$ $(1 \leq k \leq 10^6)$ &nbsp;— the length of the path of Denis.</p><p>In the next $k$ lines output pairs $v_i, t_i$ &nbsp;— pairs that describe Denis's route (as in the statement).</p><p>All route requirements described in the statements must be met.</p><p>It is guaranteed that under given restrictions there is at least one route and an answer whose length does not exceed $10^6$. If there are several possible answers, print any.</p>





```input1
5
1 2
2 3
2 4
4 5
```




```output1
13
1 0
2 1
3 2
3 1
2 2
4 3
4 1
5 2
5 1
4 2
2 3
2 0
1 1
```


