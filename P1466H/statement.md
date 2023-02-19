## Description

<div><p>Getting so far in this contest is not an easy feat. By solving all the previous problems, you have impressed the gods greatly. Thus, they decided to spare you the story for this problem and grant a formal statement instead.</p><p>Consider $n$ agents. Each one of them initially has exactly one item, <span class="tex-font-style-bf">$i$-th agent has the item number $i$</span>. We are interested in reassignments of these items among the agents. An assignment is valid iff each item is assigned to exactly one agent, and each agent is assigned exactly one item.</p><p>Each agent has a preference over the items, which can be described by a permutation $p$ of items sorted from the most to the least desirable. In other words, the agent prefers item $i$ to item $j$ iff $i$ appears earlier in the permutation $p$. A <span class="tex-font-style-bf">preference profile</span> is a list of $n$ permutations of length $n$ each, such that $i$-th permutation describes preferences of the $i$-th agent.</p><p>It is possible that some of the agents are not happy with the assignment of items. A set of dissatisfied agents may choose not to cooperate with other agents. In such a case, they would exchange the items they possess initially ($i$-th item belongs to $i$-th agent) only between themselves. Agents from this group don't care about the satisfaction of agents outside of it. However, they need to exchange their items in such a way that will make at least one of them happier, and none of them less happy (in comparison to the given assignment).</p><p>Formally, consider a valid assignment of items&nbsp;— $A$. Let $A(i)$ denote the item assigned to $i$-th agent. Also, consider a subset of agents. Let $S$ be the set of their indices. We will say this subset of agents is dissatisfied iff there exists a valid assignment $B(i)$ such that: </p><ul> <li> For each $i \in S$, $B(i) \in S$. </li><li> No agent $i \in S$ prefers $A(i)$ to $B(i)$ (no agent from the $S$ is less happy). </li><li> At least one agent $i \in S$ prefers $B(i)$ to $A(i)$ (at least one agent from the $S$ is happier). </li></ul><p>An assignment is optimal if no subset of the agents is dissatisfied. Note that the empty subset cannot be dissatisfied. It can be proven that for each preference profile, there is precisely one optimal assignment.</p><p>Example: Consider $3$ agents with the following preference profile: </p><ol> <li> $[2, 1, 3]$ </li><li> $[1, 2, 3]$ </li><li> $[1, 3, 2]$ </li></ol><p>And such an assignment: </p><ul> <li> First agent gets item $2$ </li><li> Second agent gets item $3$. </li><li> Third agent gets item $1$. </li></ul><p>See that the set of agents $\{1, 2\}$ is dissatisfied, because they can reassign their (initial) items in the following way: </p><ul> <li> First agent gets item $2$. </li><li> Second agent gets item $1$. </li><li> Third agent gets item $3$. </li></ul><p>This reassignment will make the second agent happier and make no difference to the first agent. As a result, the third agent got an item that is worse for him, but this does not prevent the set $\{1,2\}$ from being dissatisfied (he is not in this set).</p><p>The following assignment would be optimal: </p><ul> <li> First agent gets item $2$. </li><li> Second agent gets item $1$. </li><li> Third agent gets item $3$. </li></ul><p>Given an assignment $A$, calculate the number of distinct preference profiles for which assignment $A$ is optimal. As the answer can be huge, output it modulo $10^9+7$.</p><p>Two preference profiles are different iff they assign different preference permutations to any agent.</p></div><div class="input-specification"><p>In the first line of input there is an integer $n$ ($1 \leq n \leq 40$). The next line contains $n$ space separated integers, a permutation of numbers from $1$ to $n$. The $i$-th number denotes the item assigned to agent $i$ in the optimal assignment.</p></div><div class="output-specification"><p>In a single line output one non-negative integer, the number of preference profiles for which the assignment of items given in the input is optimal modulo $10^9+7$.</p></div>

## Input

<p>In the first line of input there is an integer $n$ ($1 \leq n \leq 40$). The next line contains $n$ space separated integers, a permutation of numbers from $1$ to $n$. The $i$-th number denotes the item assigned to agent $i$ in the optimal assignment.</p>

## Output

<p>In a single line output one non-negative integer, the number of preference profiles for which the assignment of items given in the input is optimal modulo $10^9+7$.</p>





```input1
2
2 1
```




```input2
3
1 2 3
```




```input3
4
2 1 3 4
```




```output1
1
```




```output2
98
```




```output3
27408
```



## Note

<p>Assignment from the first test case is optimal only for the following preference profile:</p><p>$2, 1$</p><p>$1, 2$</p><p>If any agent wants his initial item the most and is given another item, he would form a dissatisfied set. Hence the allocation is not optimal for any other preference profile.</p>
