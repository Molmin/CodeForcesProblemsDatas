## Description

<div><p>You have been hired to supervise the project of a new amusement park. The park will have a special gimmick: directed slides that can get customers from one attraction to another quickly and in an entertaining way.</p><p>The park owner has given you the current project: a list of planned attractions and a list of slides that should be built between them. However, him being a businessman, he casually envisioned the impossible: among other things, he projected a slide coming from the Haunted Castle to the Roller Coaster, another from the Roller Coaster to the Drop Tower, and a third from the Drop Tower to the Haunted Castle. As the slides can only go downhill, it is evident why this is a problem. You don't have the luxury of ignoring the laws of physics when building the park, so you have to request changes in the project. Maybe he would accept reversing the slide between the Drop Tower and the Haunted Castle?</p><p>Formally: </p><ul> <li> The <span class="tex-font-style-bf">project</span> is a list of attractions and a list of directed slides. Each slide starts at one attraction and ends at another attraction. </li><li> A <span class="tex-font-style-bf">proposal</span> is obtained from the project by reversing the directions of some slides (possibly none or all of them). </li><li> A proposal is <span class="tex-font-style-bf">legal</span> if there is a way to assign an elevation to each attraction in such a way that every slide goes downhill. </li><li> The <span class="tex-font-style-bf">cost</span> of a proposal is the number of slides whose directions were reversed. </li></ul><p>For a given project, find and report the sum of costs all legal proposals. Since this number may be large, output it modulo $998,244,353$.</p></div><div class="input-specification"><p>The first line contains two space-separated integers $n$, $m$ ($1 \leq n \leq 18$, $0 \leq m \leq n(n-1)/2$) – the number of attractions and the number of slides, respectively. The attractions are numbered $1$ through $n$.</p><p>Then, $m$ lines follow. The $i$-th of these lines contains two space-separated integers $a_i$, $b_i$ ($1 \leq a_i, b_i \leq n$) denoting a slide from $a_i$ to $b_i$. </p><p>You may assume that: </p><ul> <li> There are no self-loops. (For each $i$: $a_i \neq b_i$.) </li><li> No slide appears twice. (For all $i \neq j$: $a_i \neq a_j$ or $b_i \neq b_j$.) </li><li> No pair of attractions is connected in both directions. (The unordered pairs $\{a_i, b_i\}$ are distinct.) </li></ul></div><div class="output-specification"><p>Output one line with a single integer, the sum of costs of all legal proposals modulo $998,244,353$.</p></div><div><h2>Scoring</h2><p>Subtask 1 (7 points): $n \leq 3$</p><p>Subtask 2 (12 points): $n \leq 6$</p><p>Subtask 3 (23 points): $n \leq 10$</p><p>Subtask 4 (21 points): $n \leq 15$</p><p>Subtask 5 (37 points): no additional constraints</p></div>

## Input

<p>The first line contains two space-separated integers $n$, $m$ ($1 \leq n \leq 18$, $0 \leq m \leq n(n-1)/2$) – the number of attractions and the number of slides, respectively. The attractions are numbered $1$ through $n$.</p><p>Then, $m$ lines follow. The $i$-th of these lines contains two space-separated integers $a_i$, $b_i$ ($1 \leq a_i, b_i \leq n$) denoting a slide from $a_i$ to $b_i$. </p><p>You may assume that: </p><ul> <li> There are no self-loops. (For each $i$: $a_i \neq b_i$.) </li><li> No slide appears twice. (For all $i \neq j$: $a_i \neq a_j$ or $b_i \neq b_j$.) </li><li> No pair of attractions is connected in both directions. (The unordered pairs $\{a_i, b_i\}$ are distinct.) </li></ul>

## Output

<p>Output one line with a single integer, the sum of costs of all legal proposals modulo $998,244,353$.</p>





```input1
2 1
1 2
```




```input2
3 3
1 2
2 3
1 3
```




```output1
1
```




```output2
9
```



## Note

<p>In the first example, there are two proposals: </p><ul> <li> The slide direction is not flipped. This proposal has cost $0$. </li><li> The slide direction is flipped. This proposal has cost $1$. </li></ul> As both proposals are valid, the answer is $0 + 1 = 1$.<p>In the second example, there are eight proposals with the slide directions as follows: </p><ul> <li> $1 \rightarrow 2$, $2 \rightarrow 3$, $1 \rightarrow 3$ (cost $0$) </li><li> $1 \rightarrow 2$, $2 \rightarrow 3$, $3 \rightarrow 1$ (cost $1$) </li><li> $1 \rightarrow 2$, $3 \rightarrow 2$, $1 \rightarrow 3$ (cost $1$) </li><li> $1 \rightarrow 2$, $3 \rightarrow 2$, $3 \rightarrow 1$ (cost $2$) </li><li> $2 \rightarrow 1$, $2 \rightarrow 3$, $1 \rightarrow 3$ (cost $1$) </li><li> $2 \rightarrow 1$, $2 \rightarrow 3$, $3 \rightarrow 1$ (cost $2$) </li><li> $2 \rightarrow 1$, $3 \rightarrow 2$, $1 \rightarrow 3$ (cost $2$) </li><li> $2 \rightarrow 1$, $3 \rightarrow 2$, $3 \rightarrow 1$ (cost $3$) </li></ul><p>The second proposal is not legal, as there is a slide sequence $1 \rightarrow 2 \rightarrow 3 \rightarrow 1$. This means that the attraction $1$ has to be strictly higher than ifself, which is clearly impossible. Similarly, the seventh proposal is not legal. The answer is thus $0 + 1 + 2 + 1 + 2 + 3 = 9$.</p>
