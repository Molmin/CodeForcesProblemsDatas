## Description

<div><p>There is a computer network consisting of <span class="tex-span"><i>n</i></span> nodes numbered 1 through <span class="tex-span"><i>n</i></span>. There are links in the network that connect pairs of nodes. A pair of nodes may have multiple links between them, but no node has a link to itself.</p><p>Each link supports unlimited bandwidth (in either direction), however a link may only transmit in a single direction at any given time. The cost of sending data across a link is proportional to the square of the bandwidth. Specifically, each link has a positive weight, and the cost of sending data across the link is the weight times the square of the bandwidth.</p><p>The network is connected (there is a series of links from any node to any other node), and furthermore designed to remain connected in the event of any single node failure.</p><p>You needed to send data from node 1 to node <span class="tex-span"><i>n</i></span> at a bandwidth of some positive number <span class="tex-span"><i>k</i></span>. That is, you wish to assign a bandwidth to each link so that the bandwidth into a node minus the bandwidth out of a node is <span class="tex-span"> - <i>k</i></span> for node 1, <span class="tex-span"><i>k</i></span> for node <span class="tex-span"><i>n</i></span>, and 0 for all other nodes. The individual bandwidths do not need to be integers.</p><p>Wishing to minimize the total cost, you drew a diagram of the network, then gave the task to an intern to solve. The intern claimed to have solved the task and written the optimal bandwidths on your diagram, but then spilled coffee on it, rendering much of it unreadable (including parts of the original diagram, and the value of <span class="tex-span"><i>k</i></span>).</p><p>From the information available, determine if the intern's solution may have been optimal. That is, determine if there exists a valid network, total bandwidth, and optimal solution which is a superset of the given information. Furthermore, determine the efficiency of the intern's solution (if possible), where efficiency is defined as total cost divided by total bandwidth.</p></div><div class="input-specification"><p>Input will begin with two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 200000</span>), the number of nodes and number of known links in the network, respectively. Following this are <span class="tex-span"><i>m</i></span> lines with four integers each: <span class="tex-span"><i>f</i></span>, <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>w</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>f</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>t</i> ≤ <i>n</i>;&nbsp;<i>f</i> ≠ <i>t</i>;&nbsp;1 ≤ <i>w</i> ≤ 100;&nbsp;0 ≤ <i>b</i> ≤ 100</span>). This indicates there is a link between nodes <span class="tex-span"><i>f</i></span> and <span class="tex-span"><i>t</i></span> with weight <span class="tex-span"><i>w</i></span> and carrying <span class="tex-span"><i>b</i></span> bandwidth. The direction of bandwidth is from <span class="tex-span"><i>f</i></span> to <span class="tex-span"><i>t</i></span>.</p></div><div class="output-specification"><p>If the intern's solution is definitely not optimal, print "BAD <span class="tex-span"><i>x</i></span>", where <span class="tex-span"><i>x</i></span> is the first link in the input that violates the optimality of the solution. If the intern's solution may be optimal, print the efficiency of the solution if it can be determined rounded to the nearest integer, otherwise print "UNKNOWN".</p></div>

## Input

<p>Input will begin with two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 200000</span>), the number of nodes and number of known links in the network, respectively. Following this are <span class="tex-span"><i>m</i></span> lines with four integers each: <span class="tex-span"><i>f</i></span>, <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>w</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>f</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>t</i> ≤ <i>n</i>;&nbsp;<i>f</i> ≠ <i>t</i>;&nbsp;1 ≤ <i>w</i> ≤ 100;&nbsp;0 ≤ <i>b</i> ≤ 100</span>). This indicates there is a link between nodes <span class="tex-span"><i>f</i></span> and <span class="tex-span"><i>t</i></span> with weight <span class="tex-span"><i>w</i></span> and carrying <span class="tex-span"><i>b</i></span> bandwidth. The direction of bandwidth is from <span class="tex-span"><i>f</i></span> to <span class="tex-span"><i>t</i></span>.</p>

## Output

<p>If the intern's solution is definitely not optimal, print "BAD <span class="tex-span"><i>x</i></span>", where <span class="tex-span"><i>x</i></span> is the first link in the input that violates the optimality of the solution. If the intern's solution may be optimal, print the efficiency of the solution if it can be determined rounded to the nearest integer, otherwise print "UNKNOWN".</p>





```input1
4 5
1 2 1 2
1 3 4 1
2 3 2 1
2 4 4 1
3 4 1 2

```




```input2
5 5
2 3 1 1
3 4 1 1
4 2 1 1
1 5 1 1
1 5 100 100

```




```input3
6 4
1 3 31 41
1 5 59 26
2 6 53 58
4 6 97 93

```




```input4
7 5
1 7 2 1
2 3 1 1
4 5 1 0
6 1 10 0
1 3 1 1

```




```output1
6

```




```output2
BAD 3

```




```output3
UNKNOWN

```




```output4
BAD 4

```



## Note

<p>Although the known weights and bandwidths happen to always be integers, the weights and bandwidths of the remaining links are not restricted to integers.</p>
