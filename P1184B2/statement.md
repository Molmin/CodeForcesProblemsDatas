## Description

<div><p>Thanks to the Doctor's help, the rebels managed to steal enough gold to launch a full-scale attack on the Empire! However, Darth Vader is looking for revenge and wants to take back his gold.</p><p>The rebels have hidden the gold in various bases throughout the galaxy. Darth Vader and the Empire are looking to send out their spaceships to attack these bases.</p><p>The galaxy can be represented as an undirected graph with $n$ planets (nodes) and $m$ wormholes (edges), each connecting two planets.</p><p>A total of $s$ empire spaceships and $b$ rebel bases are located at different planets in the galaxy.</p><p>Each spaceship is given a location $x$, denoting the index of the planet on which it is located, an attacking strength $a$, and a certain amount of fuel $f$.</p><p>Each base is given a location $x$, and a defensive strength $d$.</p><p>A spaceship can attack a base if both of these conditions hold: </p><ul> <li> the spaceship's attacking strength is greater or equal than the defensive strength of the base </li><li> the spaceship's fuel is greater or equal to the shortest distance, computed as the number of wormholes, between the spaceship's planet and the base's planet </li></ul><p>Vader is very particular about his attacking formations. He requires that each spaceship is to attack at most one base and that each base is to be attacked by at most one spaceship.</p><p>Vader knows that the rebels have hidden $k$ gold in each base, so he will assign the spaceships to attack bases in such a way that maximizes the number of bases attacked.</p><p>Therefore, for each base that is attacked, the rebels lose $k$ gold.</p><p>However, the rebels have the ability to create any number of dummy bases. With the Doctor's help, these bases would exist beyond space and time, so all spaceship can reach them and attack them. Moreover, a dummy base is designed to seem irresistible: that is, it will always be attacked by some spaceship.</p><p>Of course, dummy bases do not contain any gold, but creating such a dummy base costs $h$ gold.</p><p>What is the minimum gold the rebels can lose if they create an optimal number of dummy bases?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 100$, $0 \leq m \leq 10000$), the number of nodes and the number of edges, respectively.</p><p>The next $m$ lines contain two integers $u$ and $v$ ($1 \leq u$, $v \leq n$) denoting an undirected edge between the two nodes.</p><p>The next line contains four integers $s$, $b$, $k$ and $h$ ($1 \leq s$, $b \leq 1000$, $0 \leq k$, $h \leq 10^9$), the number of spaceships, the number of bases, the cost of having a base attacked, and the cost of creating a dummy base, respectively.</p><p>The next $s$ lines contain three integers $x$, $a$, $f$ ($1 \leq x \leq n$, $0 \leq a$, $f \leq 10^9$), denoting the location, attack, and fuel of the spaceship.</p><p>The next $b$ lines contain two integers $x$, $d$ ($1 \leq x \leq n$, $0 \leq d \leq 10^9$), denoting the location and defence of the base.</p></div><div class="output-specification"><p>Print a single integer, the minimum cost in terms of gold.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 100$, $0 \leq m \leq 10000$), the number of nodes and the number of edges, respectively.</p><p>The next $m$ lines contain two integers $u$ and $v$ ($1 \leq u$, $v \leq n$) denoting an undirected edge between the two nodes.</p><p>The next line contains four integers $s$, $b$, $k$ and $h$ ($1 \leq s$, $b \leq 1000$, $0 \leq k$, $h \leq 10^9$), the number of spaceships, the number of bases, the cost of having a base attacked, and the cost of creating a dummy base, respectively.</p><p>The next $s$ lines contain three integers $x$, $a$, $f$ ($1 \leq x \leq n$, $0 \leq a$, $f \leq 10^9$), denoting the location, attack, and fuel of the spaceship.</p><p>The next $b$ lines contain two integers $x$, $d$ ($1 \leq x \leq n$, $0 \leq d \leq 10^9$), denoting the location and defence of the base.</p>

## Output

<p>Print a single integer, the minimum cost in terms of gold.</p>





```input1
6 7
1 2
2 3
3 4
4 6
6 5
4 4
3 6
4 2 7 3
1 10 2
3 8 2
5 1 0
6 5 4
3 7
5 2
```




```output1
12
```



## Note

<p>One way to minimize the cost is to build $4$ dummy bases, for a total cost of $4 \times 3 = 12$.</p><p>One empire spaceship will be assigned to attack each of these dummy bases, resulting in zero actual bases attacked.</p>
