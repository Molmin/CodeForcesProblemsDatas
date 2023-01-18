## Description

<div><p>In the intergalactic empire Bubbledom there are $N$ planets, of which some pairs are directly connected by two-way wormholes. There are $N-1$ wormholes. The wormholes are of extreme religious importance in Bubbledom, a set of planets in Bubbledom consider themselves one intergalactic kingdom if and only if any two planets in the set can reach each other by traversing the wormholes. You are given that Bubbledom is one kingdom. <span class="tex-font-style-underline">In other words, the network of planets and wormholes is a tree.</span></p><p>However, Bubbledom is facing a powerful enemy also possessing teleportation technology. The enemy attacks every night, and the government of Bubbledom retakes all the planets during the day. In a single attack, the enemy attacks every planet of Bubbledom at once, but some planets are more resilient than others. Planets are number $0,1,…,N-1$ and the planet $i$ will fall with probability $p_i$. Before every night (including the very first one), the government reinforces or weakens the defenses of a single planet.</p><p>The government of Bubbledom is interested in the following question: what is the expected number of intergalactic kingdoms Bubbledom will be split into, after a single enemy attack (before they get a chance to rebuild)? <span class="tex-font-style-underline">In other words, you need to print the expected number of connected components after every attack.</span></p></div><div class="input-specification"><p>The first line contains one integer number $N$ ($1 \le N \le 10^5$) denoting the number of planets in Bubbledom (numbered from $0$ to $N-1$). </p><p>The next line contains $N$ different real numbers in the interval $[0,1]$, specified with 2 digits after the decimal point, denoting the probabilities that the corresponding planet will fall.</p><p>The next $N-1$ lines contain all the wormholes in Bubbledom, where a wormhole is specified by the two planets it connects.</p><p>The next line contains a positive integer $Q$ ($1 \le Q \le 10^5$), denoting the number of enemy attacks.</p><p>The next $Q$ lines each contain a non-negative integer and a real number from interval $[0,1]$, denoting the planet the government of Bubbledom decided to reinforce or weaken, along with the new probability that the planet will fall.</p></div><div class="output-specification"><p>Output contains $Q$ numbers, each of which represents the expected number of kingdoms that are left after each enemy attack. Your answers will be considered correct if their absolute or relative error does not exceed $10^{-4}$. </p></div>

## Input

<p>The first line contains one integer number $N$ ($1 \le N \le 10^5$) denoting the number of planets in Bubbledom (numbered from $0$ to $N-1$). </p><p>The next line contains $N$ different real numbers in the interval $[0,1]$, specified with 2 digits after the decimal point, denoting the probabilities that the corresponding planet will fall.</p><p>The next $N-1$ lines contain all the wormholes in Bubbledom, where a wormhole is specified by the two planets it connects.</p><p>The next line contains a positive integer $Q$ ($1 \le Q \le 10^5$), denoting the number of enemy attacks.</p><p>The next $Q$ lines each contain a non-negative integer and a real number from interval $[0,1]$, denoting the planet the government of Bubbledom decided to reinforce or weaken, along with the new probability that the planet will fall.</p>

## Output

<p>Output contains $Q$ numbers, each of which represents the expected number of kingdoms that are left after each enemy attack. Your answers will be considered correct if their absolute or relative error does not exceed $10^{-4}$. </p>





```input1
5
0.50 0.29 0.49 0.95 0.83
2 3
0 3
3 4
2 1
3
4 0.66
1 0.69
0 0.36

```




```output1
1.68040
1.48440
1.61740

```


