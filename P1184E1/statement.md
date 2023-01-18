## Description

<div><p>Heidi found out that the Daleks have created a network of bidirectional Time Corridors connecting different destinations (at different times!).&nbsp;She suspects that they are planning another invasion on the entire Space and Time. In order to counter the invasion, she plans to deploy a trap in the Time Vortex, along a carefully chosen Time Corridor. She knows that tinkering with the Time Vortex is dangerous, so she consulted the Doctor on how to proceed. She has learned the following:</p><ul> <li> Different Time Corridors require different amounts of energy to keep stable. </li><li> Daleks are unlikely to use all corridors in their invasion. They will pick a set of Corridors that requires the smallest total energy to maintain, yet still makes (time) travel possible between any two destinations (for those in the know: they will use a minimum spanning tree). </li><li> Setting the trap may modify the energy required to keep the Corridor stable. </li></ul><p>Heidi decided to carry out a field test and deploy one trap, placing it along the first Corridor. But she needs to know whether the Daleks are going to use this corridor after the deployment of the trap. </p><p>She gives you a map of Time Corridors (an undirected graph) with energy requirements for each Corridor.</p><p>For a Corridor $c$, $E_{max}(c)$ is the largest $e \le 10^9$ such that if we changed the required amount of energy of $c$ to $e$, then the Daleks may still be using $c$ in their invasion (that is, it belongs to some minimum spanning tree). Your task is to calculate $E_{max}(c_1)$ for the Corridor $c_1$ that Heidi plans to arm with a trap, which is the first edge in the graph.</p></div><div class="input-specification"><p>The first line contains integers $n$ and $m$ ($2 \leq n \leq 10^5$, $n - 1 \leq m \leq 10^6$), number of destinations to be invaded and the number of Time Corridors.</p><p>Each of the next $m$ lines describes a Corridor: destinations $a$, $b$ and energy $e$ ($1 \leq a, b \leq n$, $a \neq b$, $0 \leq e \leq 10^9$).</p><p>It's guaranteed, that no pair $\{a, b\}$ will repeat and that the graph is connected&nbsp;— that is, it is possible to travel between any two destinations using zero or more Time Corridors.</p></div><div class="output-specification"><p>Output a single integer: $E_{max}(c_1)$ for the first Corridor $c_1$ from the input.</p></div>

## Input

<p>The first line contains integers $n$ and $m$ ($2 \leq n \leq 10^5$, $n - 1 \leq m \leq 10^6$), number of destinations to be invaded and the number of Time Corridors.</p><p>Each of the next $m$ lines describes a Corridor: destinations $a$, $b$ and energy $e$ ($1 \leq a, b \leq n$, $a \neq b$, $0 \leq e \leq 10^9$).</p><p>It's guaranteed, that no pair $\{a, b\}$ will repeat and that the graph is connected&nbsp;— that is, it is possible to travel between any two destinations using zero or more Time Corridors.</p>

## Output

<p>Output a single integer: $E_{max}(c_1)$ for the first Corridor $c_1$ from the input.</p>





```input1
3 3
1 2 8
2 3 3
3 1 4

```




```output1
4

```



## Note

<p>After the trap is set, the new energy requirement for the first Corridor may be either smaller, larger, or equal to the old energy requiremenet.</p><p>In the example, if the energy of the first Corridor is set to $4$ or less, then the Daleks may use the set of Corridors $\{ \{ 1,2 \}, \{ 2,3 \} \}$ (in particular, if it were set to less than $4$, then this would be the only set of Corridors that they would use). However, if it is larger than $4$, then they will instead use the set $\{ \{2,3\}, \{3,1\} \}$.</p>
